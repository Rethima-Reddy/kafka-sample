# Calculations that can be performed on data sets:

## Calulating Sum from set of data
- To calculate sum of set of numbers we have a function called ```sum()``` that will calculate the sum of data we provided. For example:
```
x<- c(1,3,4,6,4,9)
sum(x)
> 27 
```
## Calculating Mean from set of data
- To calculate mean from a set of data we have function called ```mean()``` that will return the mean of the data set provided. For example:
```
x<- c(1,3,4,6,4,9)
mean(x)
> 4.5 
```
## Calculating Median from set of data
- To calculate median from a set of data we have function called ```median()``` that will return the median of the data set provided. For example:
```
x<- c(1,3,4,6,4,9)
median(x)
> 4.
```
## Calculaing Mode from the set of data
- Their is no pre defined function to get mode from set of data. But we can create a function that can calculate the mode from the data set. The required program is as below:
```
x<- c(1,3,4,6,4,9,1,1,5)
Mode <- function(x){
  ux<- unique(x)
  ux[which.max(tabulate(match(x,ux)))]
}

mostRepeated<-Mode(x)
mostRepeated
> 1
```
- Here the ```unique()``` function finds the unique number from the set of data and ```match()``` function will compare betweeen numbers and ```tabulate()``` will store all the resuts for each unique value from the list and ```max()``` function will picks the element with highest score and will return it. 
- Now when we assign a variable to that function like ```mostRepeated``` from our example the value will be stored in it. Thus we can find the most repeated value from a set of data.

## Sorting data
- To calculate sort from a set of data we have function called ```sort()``` that will return the sort of the data set provided. For example:
```
x<- c(1,3,4,6,4,9)
sort(x)
 > 1 3 4 4 6 9
```
## Drawing a histogram from set of data
- We can pictorially represent the data we have. To present the data in the form of histogram, we can use a predefined function called ```hist()```. For example, to a draw a histogram to a dataset called mtcars which will be downloaded by default during the instalaion process of R Studio) 
```
hist(mtcars$gear, main= "Histogram for gear data in mtcars table")
```
<p align="center">
  <img src="https://raw.githubusercontent.com/Rethima-Reddy/project-group-e/master/Images/hist.png" width="500" height="350" />
</p><br>

- gear is a column in the mtcars table as you can see.
<p align="center">
  <img src="https://raw.githubusercontent.com/Rethima-Reddy/project-group-e/master/Images/data.png" width="500" height="350" />
</p><br>

## Drawing a pie chart from set of data
- We can get a pie chart from the data set we have. We can use a predefined method called ```pie()``` to draw a pie chart. For example:
```
slices <- c(10,9,5,2,4)
lablesArray <- c("Math", "Science", "Computer","Biology","history")
pie(slices,lables = lableArray, main = "Pie Chart to represent interests of students")
```
The result of this is as shown. The ```main``` is the parameter to set a title for a diagram.
(pie chart image)
<p align="center">
  <img src="https://raw.githubusercontent.com/Rethima-Reddy/project-group-e/master/Images/pie.png" width="500" height="350" />
</p><br>

## Drawing a boxPlot from set of data present
- We can draw a box plot using a predefined function called ```boxplot()```. Example is as follows:
```
boxplot(mtcars$mpg~mtcars$vs)
```
- This will plot the miles per hour for a car against its engine as shown.(img)
<p align="center">
  <img src="https://raw.githubusercontent.com/Rethima-Reddy/project-group-e/master/Images/box.png" width="500" height="350" />
</p><br>
