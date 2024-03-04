# robust-fpop

This is a fork of https://github.com/guillemr/robust-fpop which is the
main repo for this project.

## count number of intervals

```{r}
remotes::install_github("tdhock/robust-fpop@interval-count")
set.seed(1)
fit <- robseg::Rob_seg(rnorm(10), lambda=100, lthreshold=1, lslope=0)
fit$intervals
```

On my system, the code above gives the result below,

```{r}
> fit$intervals
 [1]  2  4  5  6  8  9 11 12 14 15
```
