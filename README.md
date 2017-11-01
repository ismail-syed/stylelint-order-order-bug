## Steps to reproduce

* `yarn install`
* `yarn run stylelint` reports no stylelint errors
* `yarn run stylelint:fix` applies fixes that weren't previously reported

Expected: `yarn run stylelint` to report the errors

What happened: `yarn run stylelint` did not report the errors

**Important:** When try to disable the stylelint rule in the source, the fixer will still apply the fix, even though it's disabled:

```
/* stlyleint-disable order/order */
...scss code
/* stlyleint-enable order/order */
```

I suspect this is because the lint error doesn't get report properly.
