# Society Accounts

[![Society logo](https://society-assets.s3.ca-central-1.amazonaws.com/social.network+horizontal.png)](https://social.network)

This repository is part of the source code of Society. You can find more information at [social.network](https://social.network) or by contacting support@social.network.

You can find the published source code at [github.com/social-network/society-deployer](https://github.com/social-network/society-deployer).

## society-account

> For account verifications and forgotten passwords.

## Build Instructions

1. Run `yarn`
1. Run `yarn start`
1. Open [http://localhost:8081/](http://localhost:8081/)

## Deployment

Depending on the branch name it will be automatically deployed to the following environments:

- `staging` -> `society-account-staging`

### Release flow

1. Merge staging into master
1. Create a tag with `npm version <version bump type>`. Possible values for `version bump type` are `patch`, `minor` or `major`.
1. The tag will be pushed to master and Travis will deploy the new version. Manual deployment can be triggered via `eb deploy`.
