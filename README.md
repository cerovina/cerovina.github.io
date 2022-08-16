Welcome to my data analysis projects! 📊
============================

----------------------------

----------------------------

# 1) Irises 🌸

--------------

I created a chart in R which compares the sepal length, sepal width, petal length and petal width of various iris samples.

--------------------------------------------------------------------------------------------------------------------------

![Image 1](https://github.com/cerovina/Irises-Graph/blob/main/IrisScreenshot.png?raw=true)
_Image 1: The process_

------------------------------------------------------------------------------------------

![Image2](https://github.com/cerovina/Irises-Graph/blob/main/IrisesGraph.png?raw=true)
_Image 2: The graph_

--------------------------------------------------------------------------------------

## • Sepal length _(blue)_
## • Sepal width _(red)_
## • Petal length _(green)_
## • Petal width _(purple)_

-------------------------------------------------------------------------------------------------------------------------

![Image3](https://www.integratedots.com/wp-content/uploads/2019/06/iris_petal-sepal-e1560211020463.png)
_Image 3: The flower_

--------------------------------------------------------------------------------------------------------------------------

### Conclusion:

The sepals, which are, in most flowers, usually green and smaller with a more protective role, are in this case larger than the petals, as the graph shows. Both sepals and petals are large and colourful in irises, attracting and guiding many insects to their pollen.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

### The code:

<sub>library(dplyr)</sub>
<sub>mydata <- read.csv("iris.csv")</sub>
<sub>mysubdata <- select(mydata, Sepal.Length, Sepal.Width, Petal.Length, Petal.Width, Species)</sub>
<sub>mysubdata <- mysubdata[c(1,2,3,4)]</sub>
<sub>mymatrix <- data.matrix(mysubdata)</sub>
<sub>mymatrixtrans <- t(mymatrix)</sub>
<sub>barplot(mymatrixtrans,</sub>
<sub>xlab="Iris samples",</sub>
<sub>col=c("blue","red","green","purple"))</sub>
<sub>legend("topleft",cex=0.5,c("Sepal length","Sepal width","Petal length","Petal width"),</sub>
<sub>fill=c("blue","red","green","purple"))</sub>
