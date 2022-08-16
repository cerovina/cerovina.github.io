MY DATA ANALYSIS PROJECTS 📊
============================

----------------------------

# 1) Irises 🌸

--------------

![Image 1](https://github.com/cerovina/Irises-Graph/blob/main/IrisScreenshot.png?raw=true)
_Image 1: The process_

------------------------------------------------------------------------------------------

![Image2](https://github.com/cerovina/Irises-Graph/blob/main/IrisesGraph.png?raw=true)
_Image 2: The graph_

--------------------------------------------------------------------------------------

## 1. Sepal length _(blue)_
## 2. Sepal width _(red)_
## 3. Petal length _(green)_
## 4. Petal width _(purple)_

-------------------------------------------------------------------------------------------------------------------------

I created a chart in R which compares the sepal length, sepal width, petal length and petal width of various iris samples.

--------------------------------------------------------------------------------------------------------------------------

### The code:

<sub>library(dplyr)</sub>

<sub>mydata <- read.csv("iris.csv")</sub>
          
<sub>mysubdata <- select(mydata, Sepal.Length, Sepal.Width, Petal.Length, Petal.Width, Species)</sub>
        
<sub>mysubdata <- mysubdata[c(1,2,3,4)]</sub>
             
<sub>mymatrix <- data.matrix(mysubdata)</sub>
        
<sub>mymatrixtrans <- t(mymatrix)</sub>
                 
<sub>barplot(mymatrixtrans,</sub>
                 
             xlab="Iris samples",
                 
             col=c("blue","red","green","purple"))
                 
<sub>legend("topleft",cex=0.5,c("Sepal length","Sepal width","Petal length","Petal width"),</sub>
                 
             fill=c("blue","red","green","purple"))
