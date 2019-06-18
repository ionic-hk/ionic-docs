# build-translate

this script was built by https://github.com/ionic-jp/ionic-docs for helping other developers to translate ionic-team/ionic-docs

## What is?

This script using for translate api, cli, and native document.
This can do this.

- Create editable file for translate.
- Apply translate file at build.
- Check diff from original file.


## Why?

Some Ionic document is created by resource of JSON file.

|  Type  |  Document URL  | Resource |
| ---- | ---- | ---- |
|  API  | [Components](https://ionicframework.com/docs/components) | `@ionic/docs/core.json` |
|  CLI  |  [Command Reference](https://ionicframework.com/docs/cli)  | [cli.json](https://github.com/ionic-team/ionic-docs/blob/master/scripts/data/cli.json) |
|  Native  | [Ionic Native](https://ionicframework.com/docs/native) | [native.json](https://github.com/ionic-team/ionic-docs/blob/master/scripts/data/native.json) |

This raw Ionic document is very difficult to translate as it is.

So, these JSON file are mixed with other Markdown document into the final documentation page on website.


## Usage
### Create editable file

If you wanna generates editable files from those raw Ionic document again (e.g. updating to latest version)

```shell
$ npm run translate:create
```

This command generates editable file under `src/translate/*`.
And `src/translate/.detection/*` is use for get diff from original. **don't use or add .gitignore**.


### Apply translate file

```shell
$ npm run translate
```

This command generates `script/data/translated-api.json` and `script/data/translated-cli.json` and `script/data/translated-native.json`.
This is resource file instead of original file.


## Difference from ionic-team/ionic-docs

this translate module does not exist in ionic-team/ionic-docs. If you are interested in bringing this translate module to other ionic-docs/fork, please read https://github.com/ionic-jp/ionic-docs/blob/master/scripts/build-translate/readme.md and look for `require change file` and `diff package.json`


### Get diff from original

```shell
$ ts-node -P scripts/tsconfig.json scripts/build-translate diff
```


## Sample
### Japanese Docs
[ionicframework.jp](https://ionicframework.jp)
