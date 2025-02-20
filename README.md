## Repo fork for learning. Nothing useful for thirds.

[![Code coverage badge](https://img.shields.io/badge/coverage-100%25-brightgreen)](https://stryker-mutator.io/robobar-example/reports/coverage/index.html)
[![Mutation testing badge](https://img.shields.io/endpoint?style=flat&url=https%3A%2F%2Fbadge-api.stryker-mutator.io%2Fgithub.com%2Fstryker-mutator%2Frobobar-example%2Fmaster)](https://dashboard.stryker-mutator.io/reports/github.com/stryker-mutator/robobar-example/master)


# Welcome to the RoboBar

> An introduction to mutation testing

_How code coverage of 100% could mean only 60% is tested._

## TL;DR

No time to run the example yourself? Don't worry, we did it for you. Open it right in your browser:

* [The RoboBar website](https://stryker-mutator.io/robobar-example/)
* [Coverage report](https://stryker-mutator.io/robobar-example/reports/coverage/index.html)
* [Mutation report](https://stryker-mutator.io/robobar-example/reports/mutation/html/index.html)

## What is this?
The RoboBar is a small application to demo mutation testing. It actually has a fair amount of unit tests. When we wrote this application, we didn't even try our best to write bad tests. We just focussed on code coverage and didn't practice Test Driven Development. It turns out it's really easy to write bad tests or forget a few important test cases. The RoboBar even has a fairly large bug. Finding it is pretty easy using the mutation report. Why don't you give it a try? 😁

## Try it yourself

1. Install [git](https://git-scm.com)
1. Install [nodejs](https://nodejs.org/)
1. Open command prompt and clone this repository:
   ```
   git clone https://github.com/stryker-mutator/robobar-example
   ```
1. Change directory into the robobar and install the dependencies.
   ```
   cd robobar-example
   npm install
   ```
1. Run tests with npm. This will generate a code coverage report. 
   ```
   npm test
   ``` 
1. Review the 100% code coverage score. Open up the code coverage report located in the `reports/coverage` directory.
1. Run mutation testing with [Stryker](https://stryker-mutator.io)
   ```
   npm run stryker
   ```
1. Review the 50% mutation score. Open up the mutation report located in the `reports/mutation` directory.
1. Run the website with `npm start`. Can you find the bug?

## Try to install stryker yourself.

If you want to install stryker yourself, step back in history using git:

```
git checkout e92b8d4
npm install
```

After that you can install stryker for yourself:

```js
npm i -g stryker-cli
stryker init
```

Choose the following options in the questionnaire:

* Install stryker?: `Yes`
* Test runner: `Karma`
* Test framework: `Jasmine`
* Language: `javascript`
* Transformations: *none*
* Reporters: `html, clear text, progress`

After the plugins are installed, try it out:

```
stryker run
```

