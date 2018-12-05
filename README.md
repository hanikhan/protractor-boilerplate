## How to use

- do a `git clone` of this project
- go to the root of the project and execute `npm install`
- to get the tests running make sure you have a local `webdriver-manager` running (`directConnect` from protractor has some issues)

Then there are 3 ways to run tests:

1. Run 1 or multiple featurefiles. This can be done with `npm run e2e -- --feature=example` or `npm run e2e -- --feature= example,playground`. Only provide the name of the featurefile(s) without the `.feature`
2. Run a specific tagged test(s) / featurefile(s). This can be done with `npm run e2e -- --tags=@tagName`. Please check the [docs](https://docs.cucumber.io/tag-expressions/) about how to use tags
3. Run all the available featurefiles. This can be done with `npm run e2e`

> **If you want to run tests and  nd after failure only rerun the failed ones, then use `npm run flake` to run it with `protractor-flake`**