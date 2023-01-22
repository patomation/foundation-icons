```
█▀▀ █▀█ █░█ █▄░█ █▀▄ ▄▀█ ▀█▀ █ █▀█ █▄░█   █ █▀▀ █▀█ █▄░█ █▀
█▀░ █▄█ █▄█ █░▀█ █▄▀ █▀█ ░█░ █ █▄█ █░▀█   █ █▄▄ █▄█ █░▀█ ▄█
```

This is a package containing a version of foundation icons.
Foundation Icons needed an npm module. So I took it upon my self to create this one.

## Usage

---

```
npm install foundation-icons
```

## (Optional) Install Webpack loader

```
npm install url-loader
npm install file-loader
```

Configure The WebPack Loaders

```javascript
module.exports = {
  module: {
    loaders: [
      // the url-loader uses DataUrls.
      // the file-loader emits files.
      {
        test: /\.woff(2)?(\?v=[0-9]\.[0-9]\.[0-9])?$/,
        loader:
          'url-loader?limit=10000&mimetype=application/font-woff',
      },
      {
        test: /\.(ttf|eot|svg)(\?v=[0-9]\.[0-9]\.[0-9])?$/,
        loader: 'file-loader',
      },
    ],
  },
}
```
