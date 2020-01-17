# plugin-i18n-concat
Concat all your i18n files in one file. files should be written like **(\*).i18n_(\*).json**

# Usage

* assetsPath: from where we find all the files
* fileName: name of the final json file

```bash
npm install --save-dev plugin-i18n-concat
```

```bash
const I18nPlugin = require('plugin-i18n-concat');
```

```bash
module.exports = {
    plugins: [
        new I18nPlugin({assetsPath: './dist', fileName: 'index'}),
    ]
}
```

# Sample

```bash
from: 
    * src/folder1/component1.i18n_fr.json
    * src/folder1/component1.i18n_en.json

    * src/folder2/component2.i18n_fr.json
    * src/folder2/component2.i18n_en.json

to:
    * dist/index.i18n_fr.json
    * dist/index.i18n_en.json
```
