# Day-1
Roaming


data("iris")
head(iris)

plot(iris, col=iris$Species)
summary(iris)
i<- duplicated(iris)
i
which(i)
iris[i,]
?unique
?complete.cases
clean.data<- unique(iris[complete.cases(iris),])
summary(clean.data)
aggregate(.~ Species, data = iris, FUN = mean)
aggregate(.~ Species, data = iris, FUN = median)
id <- sample(2:nrow(iris), 20)
id
iris
s <- iris[id,]
plot(s, col = s$Species)
library(sampling)
library(scatterplot3d)
scatterplot3d(iris[,1:3], color = as.integer(iris$Species))
summary(iris)
mean(iris$Sepal.Length)
sd(iris$Sepal.Length)
mean(iris$Sepal.Length, na.rm = TRUE)
