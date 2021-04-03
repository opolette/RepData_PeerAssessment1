---
title: "Activity Monitoring"
author: "OP"
date: "02/04/2021"
output: 
  html_document:
    keep_md: true
---
## Loading and preprocessing the data


## What is mean total number of steps taken per day?
![](PA1_template_files/figure-html/TotalDailySteps-1.png)<!-- -->

```
## [1] "Mean:  10766.1886792453  / Median:  10765"
```

## What is the average daily activity pattern?
![](PA1_template_files/figure-html/avgDay-1.png)<!-- -->

** There is clearly a peak of activity around mid day**

## Imputing missing values

```
## [1] "Number of NAs: 2304"
```

![](PA1_template_files/figure-html/missVal-1.png)<!-- -->

```
## [1] "Mean:  10766.1886792453  / Median:  10766.1886792453"
```
**We see that replacing NA in the the "steps" column by the mean of steps per 5mn interval does not impact the overall mean, as expected. However, the median, which was very close to the mean in the initial Dataframe, now is equal to the mean...**

## Are there differences in activity patterns between weekdays and weekends?

```
## `summarise()` has grouped output by 'dayOfWeek'. You can override using the `.groups` argument.
```

![](PA1_template_files/figure-html/weekdaysPattern-1.png)<!-- -->

**There are differences: the average number of steps during weekends is slightly lower at mid-day and higher of about 100 steps in the afternoon, per interval of 5 minutes.**
