# flashcard (q-flashcard)

A Quasar Framework app

## Install the dependencies
```bash
yarn
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)
```bash
yarn dev
```
> 如果直接使用 `quasar dev` 並搭配 Node.js 17 以上版本，會遇到 `ERR_OSSL_EVP_UNSUPPORTED`。`yarn dev` 已自動加上 `NODE_OPTIONS=--openssl-legacy-provider` 來支援較新的 Node.js／OpenSSL。

### Lint the files
```bash
yarn run lint
```

### Build the app for production
```bash
yarn build
```

### Customize the configuration
See [Configuring quasar.conf.js](https://quasar.dev/quasar-cli/quasar-conf-js).
