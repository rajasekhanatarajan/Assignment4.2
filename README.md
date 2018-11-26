# Assignment4.2
#Write a program to create barplots for all the categorical columns in mtcars.

mtcars <- c(mpg) barplot(mtcars) mtcars <- c(cyl) barplot(mtcars) mtcars <- c(disp) barplot(mtcars) mtcars <- c(hp) barplot(mtcars) mtcars <- c(drat) barplot(mtcars) mtcars <- c(wt) barplot(mtcars) mtcars <- c(qsec) barplot(mtcars) mtcars <- c(vs) barplot(mtcars) mtcars <- c(am) barplot(mtcars) mtcars <- c(gear) barplot(mtcars) mtcars <- c(carb) barplot(mtcars)

#Create a scatterplot matrix by gear types in mtcars dataset.

library(lattice) splom(mtcars[c(1,3,5,6)], groups=gear, data=mtcars, panel=panel.superpose, key=list(title="Gear Types", columns=3, points=list(pch=super.sym$pch[1:3], col=super.sym$col[1:3]), text=list(c("1 Gear","2 Gear","3 Cylinder"))))

#Write a program to create a plot density by class variable.

a <- density(mtcars$mpg) plot(a) b <- density(mtcars$cyl) plot(b) c <- density(mtcars$disp) plot(c) d <- density(mtcars$hp) plot(d) e <- density(mtcars$drat) plot(e) f <- density(mtcars$qsec) plot(f) g <- density(mtcars$vs) plot(g) h <- density(mtcars$am) plot(h) i <- density(mtcars$gear) plot(i) j <- density(mtcars$carb) plot(j)
