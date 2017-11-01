## Steps to reproduce

* `yarn install`
* `yarn run stylelint` reports no stylelint errors
* `yarn run stylelint:fix` applies fixes that weren't previously reported

Expected: `yarn run stylelint` to report the errors

What happened: `yarn run stylelint` did not report the errors
