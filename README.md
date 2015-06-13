# useful-express-partials

> A collection of useful Jade view partials for ExpressJS server: error reporting, analytics, etc.

    npm install --save useful-express-partials

From the main layout Jade file include (assuming this jade file is in views/ subfolder of the project)

```jade
doctype html
html
  head
    meta(charset='utf-8')
    title #{title}
    include ../node_modules/useful-express-partials/partials/raygun-crash-reporter
    include ../node_modules/useful-express-partials/partials/heap-analytics
  body
    include partials/header
    .container
      block content
```

## included partials

### raygun-crash-reporter

Flexible client-side crash reporting, including commit and version tags.

### heap-analytics

If the API key exists, includes the library code, plus tries to identify the user with email / name.

## Small print

Author: Gleb Bahmutov &copy; 2015
[@bahmutov](https://twitter.com/bahmutov) [glebbahmutov.com](http://glebbahmutov.com)
[glebbahmutov.com/blog](http://glebbahmutov.com/blog)

License: MIT - do anything with the code, but don't blame me if it does not work.

Spread the word: tweet, star on github, etc.

Support: if you find any problems with this module, email / tweet / open issue on Github
