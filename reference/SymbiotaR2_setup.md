# Set default URL for Symbiota2 portal download

Sets the `SymbiotaR2_url` option for you, optionally, by appending it to
your `.Rprofile`. Checks whether you've specified a valid URL that can
be reached, and attempts to pull a resource from the API, to confirm
that the URL does specify a Symbiota2 portal.

## Usage

``` r
SymbiotaR2_setup(url, append = FALSE, verbose = TRUE)
```

## Arguments

- url:

  URL of Symbiota2 portal (a trailing `/` will be appended, if it is not
  given)

- append:

  `logical` of whether to attempt to append this to your `.Rprofile`
  file, making this your default every time you start up `R`

- verbose:

  `logical` of whether or not to display output

## Value

Invisbly, the URL that has been stored

## Author

Will Pearse

## Examples

``` r
if (FALSE) { # \dontrun{
# An example (that doesn't work because it's not a real portal)
SymbiotaR2_setup("http://nonexistent-portal.com/api/")
# Trying to save a non-existence portal
SymbiotaR2_setup("http://nonexistent-portal.com/api/", TRUE)
} # }
```
