# upload-app-browserstack action

This action helps you upload your app to BrowserStack.

## Inputs

### `app-path`

**Required** The path for the app to be uploaded. Default `"Undefined"`.

### `browserstack-username`

**Required** The username for BrowserStack. Default `"Undefined"`.

### `browserstack-accesskey`

**Required** The accesskey for BrowserStack. Default `"Undefined"`.

### `custom-id`

**Optional** The custom id for BrowserStack. Default `"upload-app-browserstack"`.

## Outputs

### `browserstack-app-url`

The url for the app uploaded.

## Example usage

```
- name: Upload APK to BrowserStack
  uses: shreyanshp/upload-app-browserstack@v3
  with:
    app-path: /path-to-apk/app.apk
    browserstack-username: ${{ secrets.BROWSERSTACK_USERNAME }}
    browserstack-accesskey: ${{ secrets.BROWSERSTACK_ACCESSKEY }}
```

