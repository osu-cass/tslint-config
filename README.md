# @osu-cass/tslint-config

[![CircleCI](https://circleci.com/gh/osu-cass/tslint-config.svg?style=svg)](https://circleci.com/gh/osu-cass/tslint-config) ![npm (scoped)](https://img.shields.io/npm/v/@osu-cass/tslint-config.svg) [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

This package contains the baseline rules for TypeScript projects at the Oregon State University [Center for Applied Systems and Software](http://cass.oregonstate.edu/). It extends the following other shareable configurations:

- [Airbnb](https://www.npmjs.com/package/tslint-config-airbnb)
- [Prettier](https://www.npmjs.com/package/tslint-config-prettier)
- [Microsoft Contrib](https://www.npmjs.com/package/tslint-microsoft-contrib)

## Usage

When starting a new project, all first you need to install the package and its dependencies:

```sh
# In your project directory
npm i -D typescript tslint tslint-language-service @osu-cass/tslint-config

# Make a TSLint config file in the same directory
echo '{ "extends": ["@osu-cass/tslint-config"] }' > tslint.json
```

If you'd rather instanciate the `tslint.json` yourself, here are the contents:
```json
{
    "extends": ["@osu-cass/tslint-config"]
}
```

You should be good to go. Open an issue if you have any problems.

## Updating this config

If you want to change any of the rules, either fork this repo and create a Pull Request, or (if you're a contributor) make a branch and a PR. Once your changes have been merged into `master`, it will be released automatically.

We enforce the use of [Conventional Commits](https://conventionalcommits.org/) via [Commitlint](https://github.com/marionebl/commitlint), so make sure you're using them as you contribute. [Semantic Release](https://github.com/semantic-release/semantic-release) relies on the types of these commits to correctly increment the release number.

You can check out the NPM page when it's released: https://www.npmjs.com/package/@osu-cass/tslint-config
