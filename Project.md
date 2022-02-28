Project
================
Alexa Kraklau, Sara Knight
2/28/2022

Our topic is based from a previous Tidy Tuesday data set of all Scooby
Doo television show episodes and movies.
<https://github.com/rfordatascience/tidytuesday/blob/master/data/2021/2021-07-13/readme.md>
For each observation there are many variables including the monster, the
person under the mask, the member who unmasked them, etc. Since neither
one of us has a lot of R experience, we thought this would be a good
data set to look at because it has several quanitative and categorical
variables that we are able to analyse.

We plan to create graphical displays of certain variables to identify
the efficacy of Mystery Inc as well as the individual members. There are
also other directions we could go such as mapping locations or
generating episode combinations.

``` r
scoobydoo <- readr::read_csv('https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2021/2021-07-13/scoobydoo.csv')
```

    ## 
    ## ── Column specification ────────────────────────────────────────────────────────
    ## cols(
    ##   .default = col_character(),
    ##   index = col_double(),
    ##   date_aired = col_date(format = ""),
    ##   run_time = col_double(),
    ##   monster_amount = col_double(),
    ##   unmask_other = col_logical(),
    ##   caught_other = col_logical(),
    ##   caught_not = col_logical(),
    ##   suspects_amount = col_double(),
    ##   culprit_amount = col_double(),
    ##   door_gag = col_logical(),
    ##   batman = col_logical(),
    ##   scooby_dum = col_logical(),
    ##   scrappy_doo = col_logical(),
    ##   hex_girls = col_logical(),
    ##   blue_falcon = col_logical()
    ## )
    ## ℹ Use `spec()` for the full column specifications.
