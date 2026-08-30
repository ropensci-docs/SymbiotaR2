# Retrieves Occurrence resources from the Symbiota2 server

Functions that retrieve Occurrence resources from the server previously
connected to. Each function either retrieves an individual resource or a
page of resources, depending on the arguments provided.

## Usage

``` r
AccessStats(id, page, url = NULL)

Determinations(id, page, url = NULL)

Duplicates(id, page, url = NULL)

EditLocks(id, page, url = NULL)

Edits(id, page, url = NULL)

FullText(id, page, url = NULL)

GuidDeterminations(id, page, url = NULL)

GuidOccurrences(id, page, url = NULL)

LookupChronostratigraphy(id, page, url = NULL)

LookupCounties(id, page, url = NULL)

LookupCountries(id, page, url = NULL)

LookupStateProvinces(id, page, url = NULL)

UploadMappings(id, page, url = NULL)

UploadParameters(id, page, url = NULL)

Verification(id, page, url = NULL)

Associations(id, page, url = NULL)

Comments(id, page, url = NULL)

DatasetLink(id, page, url = NULL)

Datasets(id, page, url = NULL)

Exchange(id, page, url = NULL)

Loans(id, page, url = NULL)

Occurrences(id, page, url = NULL)
```

## Arguments

- id:

  id value (usually `numeric`, but not always) used to refer to the
  specific resource to pull from the database

- page:

  `numeric` value referring to the page of resources to pull. If neither
  an id or a page parameter is provided, function will pull the first
  page of resources (i.e. `page=1`)

- url:

  URL string of the Symbiota2 portal to be connected to. A trailing `/`
  will be appended, if it is not given.

## Value

If using `id`, the specific resource specified; if using page, the
`page` specified of resources

## Note

To specify a default URL to refer to, see
[`SymbiotaR2_setup()`](https://docs.ropensci.org/SymbiotaR2/reference/SymbiotaR2_setup.md)

## Author

Austin Koontz

## Examples

``` r
if (FALSE) { # \dontrun{
# Pulling a page of Occurrences, from a (nonexistent) dummy portal
entries <- Occurrence(page = 6, url = "http://dummy-portal.com/api/")
} # }
```
