[![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/0.1.0/active.svg)](http://www.repostatus.org/#active)
[![Is the package on CRAN?](http://www.r-pkg.org/badges/version/assertive.data.us)](http://www.r-pkg.org/pkg/assertive.data.us)
[![SemaphoreCI Build Status](https://semaphoreci.com/api/v1/projects/536880e1-f50c-40ac-b021-7e81aa55afab/635106/badge.svg)](https://semaphoreci.com/richierocks/assertive-data-us)
[![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/nr5ii01ko093ygtx?svg=true)](https://ci.appveyor.com/project/richierocks/assertive-data-us)
[![Research software impact](http://depsy.org/api/package/cran/assertive.data.us/badge.svg)](http://depsy.org/package/r/assertive.data.us)

# assertive.data.us

A set of predicates and assertions for checking the properties of US-specific complex data types.  Most of the documentation is on the *[assertive](https://bitbucket.org/richierocks/assertive)* page.  End-users will usually want to use *assertive* directly.


### Installation

To install the stable version, type:

```{r}
install.packages("assertive.data.us")
```

To install the development version, you first need the *devtools* package.

```{r}
install.packages("devtools")
```

Then you can install the *assertive.data.us* package using

```{r}
library(devtools)
install_bitbucket("richierocks/assertive.data.us")
```

### Predicates

`is_us_telephone_number` checks character vectors for UK telephone numbers.

`is_uk_zipcode` checks character vectors for UK zip codes.

### Assertions

Predicates all return a vector and have two corresponding assertions.  For example,
`is_us_telephone_number` has `assert_all_are_us_telephone_numbers` and `assert_any_are_us_telephone_numbers`.