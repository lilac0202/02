# Load the dataset
 data (mtcars)
 head (mtcars)
 # scatter plot
 plot (mtcars$mpg, mtcars$hp,
    main = "MPG vs Horsepower",
    xlab = "Miles per Gallon (mpg)",
    ylab = "Horsepower (hp)",
    col = "blue",
    pch = 19)
 # histogram
 hist (mtcars$mpg,
    main = “Histogram of Miles per Gallon (MPG)",
    xlab = "Miles per Gallon (mpg)",
    col = "lightblue",
    border = "black",
    breaks = 10)
 # box plotrs
 boxplot (mpg ~ cyl,
    data = mtcars,
    main = "MPG by Number of Cylinders",
    xlab = "Number of Cylinders",
    ylab = "Miles per Gallon (mpg)",
    col = c("lightgreen", "lightblue", "lightcoral"))
 avg_mpg by cyl <- tapply(mtcars$mpg, mtcars$cyl, mean)
 # bar plot
 barplot (avg_mpg_by cyl,
    main = "Average MPG by Number of Cylinders",
    xlab = "Number of Cylinders",
    ylab = "Average Miles per Gallon (mpg)",
    col = "lightblue",
    border = “black")
 # Modify
 plot (mtcars$mpg, mtcars$Shp,
    main = "MPG vs Horsepower (Customized)",
    xlab = "Miles per Gallon (mpg)",
    ylab = “Horsepower (hp)",
    col = "green",
    pch = 19,
    xlim = c(10, 35), # Custom X-axis limits
    ylim = c(50, 350)) # Custom Y-axis limits
