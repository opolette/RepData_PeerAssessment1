---
title: "PA1_template"
author: "OP"
date: "02/04/2021"
output: 
  html_document:
    keep_md: true
---


# Total Number of Steps per Day
![](PA1_template_files/figure-html/TotalDailySteps-1.png)<!-- -->

```
## [1] "Mean:  10766.1886792453  / Median:  10765"
```

# Average daily activity pattern
![](PA1_template_files/figure-html/avgDay-1.png)<!-- -->

# Imputing missing values

```
## [1] "Number of NAs: 2304"
```

![](PA1_template_files/figure-html/missVal-1.png)<!-- -->

```
## [1] "Mean:  10766.1886792453  / Median:  10766.1886792453"
```
We see that replacing NA in the the "steps" column by the mean of steps per 5mn interval does not impact the overall mean, as expected. However, the median, which was very close to the mean in the initial Dataframe, now is equal to the mean...

# Are there differences in activity patterns between weekdays and weekends?

```
## `summarise()` has grouped output by 'dayOfWeek'. You can override using the `.groups` argument.
```

![](PA1_template_files/figure-html/weekdaysPattern-1.png)<!-- -->
