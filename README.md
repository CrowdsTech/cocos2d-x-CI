# cocos2d-x-CI [![Build Status: CI](https://github.com/CrowdsTech/cocos2d-x-CI/workflows/CI/badge.svg)](https://github.com/CrowdsTech/cocos2d-x-CI/actions)

# cocos2d-x-CI
GitHub Actions Workflow for building cocos2d-x 4.0 based projects

This [CI workflow](.github/workflows/ci.yml) downloads the released [4.0 tag of the cocos2d-x repository](https://github.com/cocos2d/cocos2d-x/releases/tag/cocos2d-x-4.0), creates a new hello world app with `cocos` CLI, patches generated sources in a few places and builds them on macOS, iOS, Linux and Android.

In order to replicate the same behavior in your own repo, you will need to follow the instructions in [Installing an Apple certificate on macOS runners for Xcode development](https://docs.github.com/en/actions/deployment/installing-an-apple-certificate-on-macos-runners-for-xcode-development) to enable app signing on iOS. After this your repo should contain the following secrets: `BUILD_CERTIFICATE_BASE64`, `BUILD_PROVISION_PROFILE_BASE64`, `KEYCHAIN_PASSWORD`, `P12_PASSWORD` as described in the instructions as well as `DEVELOPMENT_TEAM`, which is added by us(you can find it on your [Apple Developer account](https://developer.apple.com/account/#/membership) as the last part of the URL after you log in)

## License
Distributed under [MIT License](LICENSE)

## Contributions
Are always welcome!
