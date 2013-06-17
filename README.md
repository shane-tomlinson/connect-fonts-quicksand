# connect-fonts-quicksand

Quicksand fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-quicksand");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/quicksand-bold.otf/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/quicksand-bold.otf,quicksand-bold,quicksand-bolditalic.otf,quicksand-bolditalic,quicksand-italic.otf,quicksand-italic,quicksand-light.otf,quicksand-light,quicksand-lightitalic.otf,quicksand-lightitalic,quicksand-regular.otf,quicksand-regular/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* quicksand-bold.otf
* quicksand-bold
* quicksand-bolditalic.otf
* quicksand-bolditalic
* quicksand-italic.otf
* quicksand-italic
* quicksand-light.otf
* quicksand-light
* quicksand-lightitalic.otf
* quicksand-lightitalic
* quicksand-regular.otf
* quicksand-regular

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/quicksand-bold.otf/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin
* en

5. Set your CSS up to use the new font by using the "Quicksand" font-family.
```
    body {
      font-family: 'Quicksand', 'sans-serif', 'serif';
    }
```

## Font Info
Quicksand

* Copyright: Copyright (c) 2011, Andrew Paglinawan (www.andrewpaglinawan.com), with Reserved Font Name "Quicksand".
* Trademark: Quicksand Bold is a trademark of the Andrew Paglinawan.
* Designer: Andrew Paglinawan
* Designer URL: www.andrewpaglinawan.com 
* Vendor: Andrew Paglinawan

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-quicksand
* Repo: https://github.com/shane-tomlinson/connect-fonts-quicksand

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* https://github.com/stomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 1.1 of the SIL Open Font License

  http://scripts.sil.org/OFL

