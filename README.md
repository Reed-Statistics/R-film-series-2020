#### **Note (March 13th): We have decided to cancel the remaining R Film Series sessions out of an abundance of caution related to the coronavirus (COVID-19). However, we still encourage checking out the remaining talks!**

<p align="center">
  <img width="460" src="R-graphic.png">
</p>

* * *

Please join Tuesday from 12 - 1 pm this spring for screenings of excellent talks from the recent [Rstudio::conf](https://rstudio.com/conference/). We'll be meeting in **Physics 123**. Many/most of these talks have useful gems even to folks with only limited exposure to programming and R.

Come for the talks, stay for the follow-up conversation (and free pizza)!

* * *

#### Community Work in Data Science - March 3rd
[Data science education as an economic and public health intervention in East Baltimore](https://resources.rstudio.com/rstudio-conf-2020/data-science-education-as-an-economic-and-public-health-intervention-in-east-baltimore-jeff-leek) - Jeff Leek  

[The development of "datos" package for the R4DS Spanish translation](https://resources.rstudio.com/rstudio-conf-2020/the-development-of-datos-package-for-the-r4ds-spanish-translation-riva-quiroga-2?prevItm=0&prevCol=6275649&ts=58869) - Riva Quiroga

* * *

#### Debugging - March 10th
[Object of type ‘closure’ is not subsettable](https://resources.rstudio.com/rstudio-conf-2020/object-of-type-closure-is-not-subsettable-jenny-bryan) - Jenny Bryan

Let's try to work through some other common errors using Jenny's techniques. This function can be used to explore the `iris` dataset.

``` r
find_max <- function(x,y){
  temp <- subset(iris, Species = x)
  temp2 <- apply(temp, 2, max)
  temp2[y]
}

find_max("setosa", "Sepal.Length")
#> Sepal.Length 
#>        "7.9"
```

This next line errors out, though… you might already know why, but try using `traceback()`, `options(error = recover)`, and `browser()` to get a sense for how the different debugging functions work and track down the error.

``` r
find_max("setosa", "Sepal.Length") - find_max("versicolor", "Sepal.Length")
#> Error in find_max("setosa", "Sepal.Length") - find_max("versicolor", "Sepal.Length"): non-numeric argument to binary operator
```

How about this one?

``` r
find_max("setosa", list(1, 2))
#> Error in temp2[y]: invalid subscript type 'list'
```

<sup>Created on 2020-03-10 by the [reprex package](https://reprex.tidyverse.org) (v0.3.0.9001)</sup>

* * *

#### ~~Data Visualization - March 17th~~
[Effective Visualizations](https://resources.rstudio.com/rstudio-conf-2020/effective-visualizations-miriah-meyer) - Miriah Meyer

[Glamour of Graphics](https://resources.rstudio.com/rstudio-conf-2020/the-glamour-of-graphics-william-chase) - Will Chase

* * *

#### No Session, Spring Break! - March 24th

* * *

#### ~~Visualizing Equitable AI - March 31st~~
[Data, visualization, and designing AI](https://resources.rstudio.com/rstudio-conf-2020/data-visualization-and-designing-ai-fernanda-viegas-and-martin-wattenberg) - Fernanda Viegas \& Martin Wattenberg

* * *

#### ~~Career Advice For Aspiring Data Scientists - April 7th~~
[Career Advice for Aspiring Data Scientists](https://resources.rstudio.com/rstudio-conf-2020/panel-career-advice-for-data-scientists-jen-hecht) - Gabriela de Queiroz, David Keyes, Sydeaka Watson, \& Jen Hecht 

* * *

#### ~~Designing with RMarkdown - April 14th~~
[Of Teacup Giraffes and RMarkdown](https://resources.rstudio.com/rstudio-conf-2020/of-teacups-giraffes-and-r-markdown-desiree-de-leon) - Desirée De Leon

[RMarkdown Driven Development](https://resources.rstudio.com/rstudio-conf-2020/rmarkdown-driven-development-emily-riederer) - Emily Reiderer 
