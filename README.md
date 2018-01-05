<p align="center">
<img src="https://raw.githubusercontent.com/idancali/lali/master/logo.png" width="256px">
</p>

<h1 align="center">
Lali <br/>
The Local Amorphous Link Installer  
</h1>

## Summary

[![Module](https://img.shields.io/npm/v/lali.svg)](https://www.npmjs.com/package/lali)
[![Build](https://circleci.com/gh/idancali/lali.svg?style=svg)](https://circleci.com/gh/idancali/lali)
[![Coverage](https://api.codeclimate.com/v1/badges/3218ab8690250b0aeeba/test_coverage)](https://codeclimate.com/github/idancali/lali/test_coverage)
[![Maintainability](https://api.codeclimate.com/v1/badges/3218ab8690250b0aeeba/maintainability)](https://codeclimate.com/github/idancali/lali/maintainability)
[![Style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com)

Lali helps you install amorphous links locally. Lali understands an amorphous link as being a remote Tar GZip archive.

## Basic Usage

```
// Import Lali with default options
const lali = require('lali')

// Install an amorphous link locally
lali.link(<a .tar.gz link>).install(<local path>)
     .then(() => {
       // Link data is now available locally
     })
     .catch((error) => {
       // Something went wrong and the link was not installed
     })
```

## Code Quality

Lali is well tested and releases are not published unless the coverage is in the high 90s.

[![Test Coverage](https://api.codeclimate.com/v1/badges/3218ab8690250b0aeeba/test_coverage)](https://codeclimate.com/github/idancali/lali/test_coverage)
[![Maintainability](https://api.codeclimate.com/v1/badges/3218ab8690250b0aeeba/maintainability)](https://codeclimate.com/github/idancali/lali/maintainability)

### Unit Tests

<a href="https://circleci.com/gh/idancali/lali"> <img src="https://circleci.com/gh/idancali/lali.svg?style=svg"> </a>

```
  ✓ check if a link exists
  ✓ detect if an invalid link does not exist
  ✓ detect if a link does not exist
  ✓ fail to download a link
  ✓ successfully install a link
```

## Dependencies

Lali makes use of the following libraries:

* [got](https://github.com/sindresorhus/got) - for remote calls
