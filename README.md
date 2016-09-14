# assignment1





###Question: 1) no. of KM travelled before each stop
####Answer

```r
r <- diff(distance)
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
### Question: 3) total number of KMs travelled using min() and max()
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
# Question: 4) total number of KMs travelled using indices of vector
## Answer

```r
mi <- r[1]
mx <- r[length(r)]
tot <- mx - mi 
tot
```

```
## [1] -11
```
# Question : 5) total number of KMs travelled using rev()
## Answer

```r
a <- rev(r)
sum(a)
```

```
## [1] 2136
```

# total number of KMs travelled using head() and tail()

```r
x <- head(r)
y <- tail(r)
tot_h_t <- x+y
```
# total number of KMs travelled using head() and rev()

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
