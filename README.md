# @osu-cass/tslint-config

[![CircleCI](https://circleci.com/gh/osu-cass/tslint-config.svg?style=svg)](https://circleci.com/gh/osu-cass/tslint-config) ![npm (scoped)](https://img.shields.io/npm/v/@osu-cass/tslint-config.svg) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

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
