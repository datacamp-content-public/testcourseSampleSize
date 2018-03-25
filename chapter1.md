---
title: Template Chapter 1
description: >-
  This is a template chapter.


---
## Ex 1.1

```yaml
type: NormalExercise
lang: r
xp: 100
skills: 1
key: b3b3f3fa1a
```

Do some data science.

`@instructions`


`@hint`



`@sample_code`
```{r}
# create a pool of 1 million balls, half white and half black (Generate a vector called "pool" that represents the null hypothesis condition)
pool <- "REPLACETHIS"

# create a single sample that contains 100 balls randomly chosen from the pool

pool.samp <- "REPLACETHIS"

# calculate proportion of red balls in the single sample

prop.red.sample <- "REPLACETHIS"

table(pool.samp)

prop.red.sample

```
`@solution`
```{r}
# create a pool of 1 million balls, half white and half black (Generate a vector called "pool" that represents the null hypothesis condition)
total.n.balls <- 100000
pool <- rep(c("Red", "Black"), total.n.balls/2)

# create a single sample that contains 100 balls randomly chosen from the pool
pool.samp <- pool[sample(1:total.n.balls, 100)]

# calculate proportion of red balls in the single sample
prop.red.sample <- sum(pool.samp == "Red")/100

table(pool.samp)

prop.red.sample
```





