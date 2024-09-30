# expo-monorepo

Test out `.easignore` to only upload files needed.

- Open this repo in github codespaces
- run command to initialize
- run command to test which files are uploaded

## Initialize

```
npm install -g eas-cli

yarn install
```

### See what is uploaded to eas

https://github.com/expo/fyi/blob/main/eas-build-archive.md
```
cd apps/cool-app

rm -rf /tmp/eas-output

eas build:inspect --platform android --stage archive --output /tmp/eas-output --profile production

tree /tmp/eas-output
```

### One line
```
rm -rf /tmp/eas-output && eas build:inspect --platform android --stage archive --output /tmp/eas-output --profile production && tree /tmp/eas-output
```

### monorepo setup
https://docs.expo.dev/guides/monorepos/

