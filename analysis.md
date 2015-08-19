---
title: "Session 1"
output: html_document
---

Note: This is written using Rmarkdown. You can produce HTML and Pdf documents using Rmarkdown and Rstudio. Think documentation, reports, ppt.

The dataset we will work on today is a fun dataset. IMDB Movies. Please go ahead and download the data folder in your project directory. [Download from here](https://drive.google.com/open?id=0B9NCHJOuElCGfllXSFJsd2dFWVdabEdjQVJHSmpKaUVfZUw3VTM1NFMyT0Z6dlIzSVM1MGM)

## Read the data

Common formats I know about in Biology - Flat files  - tsv, csv, txt, <some random extension of a tab delimited file>, xlsx/xls
You don't have Databases SQL, JSON etc..

###Two recommended packages 

1. `readr` and `read_xl` for readability and concise
2. `data.table::fread` for performance and consistency



```r
library(readr)
```

```
## Error in library(readr): there is no package called 'readr'
```

```r
titles_df = read_csv("~/code/personal/pycon-pandas-tutorial/data/titles.csv")
```

```
## Error in eval(expr, envir, enclos): could not find function "read_csv"
```

```r
cast_df = read_csv("~/code/personal/pycon-pandas-tutorial/data/cast.csv")
```

```
## Error in eval(expr, envir, enclos): could not find function "read_csv"
```

```r
rel_dates_df = read_csv("~/code/personal/pycon-pandas-tutorial/data/release_dates.csv")
```

```
## Error in eval(expr, envir, enclos): could not find function "read_csv"
```

That was easy right!




```r
str(rel_dates_df)
```

```
## Error in str(rel_dates_df): object 'rel_dates_df' not found
```

```r
library(ggplot2)
qplot(rel_dates_df$year)
```

```
## Error in eval(expr, envir, enclos): object 'rel_dates_df' not found
```


