# assignment1





###Question: 1) no. of KM travelled before each stop
####Answer

```r
r <- diff(c(65311,65624,65908,66219,66499,66821,67145,67447))
r
```

```
## [1] 313 284 311 280 322 324 302
```
###Question: 2) total number of KMs travelled 
####Answer 

```r
total_kms_travld <- sum(r) 
total_kms_travld
```

```
## [1] 2136
```
###Question: 3) total number of KMs travelled using min() and max()
####Answer 

```r
mini <- min(r)
maxi <- max(r)
total_travelld <- maxi - mini 
total_travelld
```

```
## [1] 44
```
###Question: 4) total number of KMs travelled using indices of vector
####Answer

```r
mi <- r[1]
mx <- r[length(r)]
tot <- mx - mi 
tot
```

```
## [1] -11
```
###Question : 5) total number of KMs travelled using rev()
####Answer

```r
a <- rev(r)
sum(a)
```

```
## [1] 2136
```

###Question : 6) total number of KMs travelled using head() and tail()
####Answer

```r
x <- head(r)
y <- tail(r)
tot_h_t <- x+y
```
### Question : 7) total number of KMs travelled using head() and rev()
#### Answer

```r
x <- head(r)
y <- rev(r)
tot <- x+y
```

```
## Warning in x + y: longer object length is not a multiple of shorter object
## length
```

```r
tot
```

```
## [1] 615 608 633 560 633 608 626
```


```r
barplot(r)
```

![plot of chunk unnamed-chunk-8](figure/unnamed-chunk-8-1.png)
