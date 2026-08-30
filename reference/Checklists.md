# Retrieves Checklists resources from the Symbiota2 server

Functions that retrieve Checklist resources from the server previously
connected to. Each function either retrieves an individual resource or a
page of resources, depending on the arguments provided.

## Usage

``` r
ChecklistProjects(id, page, url = NULL)

Coordinates(id, page, url = NULL)

TaxaLink(id, page, url = NULL)

Checklists(id, page, url = NULL)
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
# Pulling a Coordinates resource (id = 1), from a (nonexistent) dummy portal
object <- Coordinates(id = 1, url = "http://dummy-portal.com/api/")
} # }
```
