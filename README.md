# Example package

<!-- badges: start -->
<!-- badges: end -->

Here's an example package made with litr where both its pkgdown website and its bookdown are nicely rendered.

- Its pkgdown website: https://jacobbien.github.io/example/

- Its bookdown: https://jacobbien.github.io/example/create/

To create this, we ran the following from an R console:

``` r
litr::render("index.Rmd")
fs::dir_copy("_book", "docs/create", overwrite = TRUE)
fs::dir_delete("_book")
```

We would run the above whenever we make a change.

Initial setup (done only once): On the github page for this repo, we clicked Settings > Pages and set this to be deployed from the main and then chose the /docs directory (rather than the root).