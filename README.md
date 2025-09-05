# Reproducible Research — Project 1

This repository contains my submission for **Project 1** of the *Reproducible Research* course in the [Johns Hopkins Data Science Specialization on Coursera](https://www.coursera.org/specializations/jhu-data-science).

---

## 📂 Repository Contents

- `Reproducible_Project1.Rmd` — R Markdown file with all analysis and code.
- `Reproducible_Project1.html` — knitted HTML report for submission.
- `activity.csv` — activity monitoring dataset (not tracked in Git if too large).
- `figures/` — directory for exported plots (optional).

---

## 📊 Dataset

The dataset is collected from a personal activity monitoring device, recording the number of steps taken in 5-minute intervals each day during October and November 2012.

- **steps**: Number of steps taken in a 5-minute interval (may be NA)  
- **date**: Date of the observation (YYYY-MM-DD)  
- **interval**: Identifier for the 5-minute interval (e.g. 0, 5, 10, …, 2355)  

Source: [Course data zip file](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip)

---

## 📑 Tasks Completed

1. **Loading and preprocessing the data**
   - Read CSV, cleaned dates, handled missing values.
2. **Total steps per day**
   - Histogram, mean, and median.
3. **Daily activity pattern**
   - Time series of average steps per 5-minute interval; identified peak interval.
4. **Imputing missing values**
   - Replaced NAs with mean of that interval; compared distributions before/after.
5. **Weekday vs Weekend patterns**
   - Created factor variable (weekday/weekend); compared activity with panel plots.

---

## ⚙️ Reproducibility

### Requirements
- R (≥ 4.0)
- Packages: `tidyverse`, `lubridate`, `knitr`

### Run Analysis
```r
# Knit the report
rmarkdown::render("Reproducible_Project1.Rmd")
