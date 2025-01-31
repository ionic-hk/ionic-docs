# Ionic Framework Documentation Traditional Chinese Version 繁體中文版 (unofficial)

__\*\*This is not official Ionic Team translation repositor\*\*__

you can refer to this forum thread about the translation work discussion: https://forum.ionicframework.com/t/chinese-introductions/166287


## Local Preview

First time setup please run the following to install all dependencies:

```
$ npm install
```

Run the following command the start the web app:

```
$ npm start
```

When the startup is completed, http://localhost:3333/docs/ starts up automatically.


## File Structure

- Content files are in Markdown (.md) format
- src/pages/intro.md will be displayed as /docs/intro on the website

if you are translating API, CLI and Native pages, please be aware that they require special processing. they are a mix of .json and .md files inside /src/translate/api, /src/translate/cli and /src/translate/native.

They were first generated dynamically from several .json source files, and the detail reason behind is written [/scripts/build-translate/readme.md](https://github.com/ionic-hk/ionic-docs/blob/master/scripts/build-translate/readme.md). If you are updating those .json source files to latest version, follow that readme and look for the `npm run translate:create` part.


## Wanna Contribute ?

__Appreciate Your Help__

In order to maintain the translation pages up-to-date, it requires huge effort. If you are interested in helping, please contact tatonlto@gmail.com.


__Workflow__

1. Fork this repository
2. Create an issue for translation work
3. Translate
4. Create a pull request

- [Contributing Guide](https://github.com/ionic-hk/ionic-docs/blob/master/CONTRIBUTING.md) :flashlight:
- [Project Board](https://github.com/ionic-team/ionic-docs/projects/3) :pushpin:


## Precaution

- This repository is under Apache License. Please note that your translation work is also licensed under the same license.