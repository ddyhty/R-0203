#02 practice
2:6 + 3:7

c(4,6,8,9,7)+c(6,8,9,8,6)

x <- c(0.5, 0.6) 
x <- c(TRUE, FALSE)
x <- c(T, F)
x <- c("a")
x <- c(9:26) 
x <- c(1+0i, 2+4i) 
x <- c(1+0*i, 2+4*i) 

sum(1:99)
median(1:33)
mean(1:79)

sum(2,5,7,8,9)
median(2,5,7,8,9)
median(5,5,7,8,9)
mean(2,5,7,8,9)
mean(5,5,7,8,9)

c(3,5,7,9,11,34)-2
-1:6 * 1:8
2:13 /5
abs(7)
abs(-4)
sqrt(7)

log(100)
log10(100)
log(100,10)
log(9,3)
log10(1000)
1.8e9
identical(3*3,3+3)

pi
sin(pi/3)
sin(pi/2)
sin(0)
sin(10)
cos(0)
cos(c(0,pi/4,pi/3,pi/2,pi))
round(pi,4)
floor(4.4865464)
ceiling(pi)
trunc(pi)
factorial(7)
exp(pi*1i) +1
factorial(9)+factorial(3) -78*3
choose(2,0:5)

c(4,6-2,3+1,6) == 4
4:7 != 3:6
3:6 == 3:6
exp(4:9)<1000
(4:9) *9 >= 56

sqrt(3)^2 == 3
sqrt(3)^2 -3

all.equal(sqrt(3)^2,3)
all.equal(sqrt(3)^2,6)
isTRUE(all.equal(sqrt(3)^2,6))
isTRUE(all.equal(sqrt(3)^2,3))

c("23","44","dog")=="32"
c("A","B","C","D","F")<"C"
c("a","b","c","d")>"a"    

x <- 3:6
y = 3:6
x +y*3-56

c(Inf+3,Inf-5,Inf+Inf,Inf-Inf)
c(1/Inf,Inf/1,Inf/Inf,Inf*Inf)
c(sqrt(Inf),sin(Inf),cos(Inf))
c(NA+3,NA/NA,NA*4,NA/Inf)
c(NA+NA,NA+NaN,NaN+NaN,NaN+NA)

x3 <-c(0,Inf,NaN,NA)
is.finite(x3)
is.nan(x3)
is.na(x3)

x4<-1:10>=5
!x4
y4<-1:10%%2 ==0
x4&y4

#02 answer
Q1：用于整数除法的操作符是什么？
A1：%/%

Q2：如何检查变量X是否等于pi？
A2：使用all_equal

Q3:至少描述两种给变量赋值的方式
A3：如x<-5,是将5赋值给x
X=3，是将3赋值给x

Q4：这5个数值中哪些是无限值？
A4：lnf和-lnf

Q5：这5个数值中哪些不是缺失值？
A5：0，NaN ,lnf和-lnf

#02练习1
#1)
atan(1/(1:1000)）
#2）
x <- c(1:1000)
y <-  atan(1/x)
z <- (1/ tan(y))

练习2
x==z

identical(x,z)

all-equal(x,z)

all-equal(x,z,0)

练习3
true_and_missing <- c(TRUE,NA)
false_and_missing<- c(FALSE,NA)
mixed <-c(TRUE,FALSE,NA)
any(true_and_missing,false_and_missing,mixed)
all(true_and_missing,false_and_missing,mixed)



#03 practice
class(c(TRUE,FALSE))
class(sqrt(1:7))
class(3+5i)
class(3)
class(3L)
class(2.5:8.5)
class(3:7)

class(c("ewer","she","dfgvf"))

(gender <- factor(c("male","female","male","female")))
levels(gender)
nlevels(gender)
(grade <- factor(c("primary","middle","high","high")))
levels(grade)
nlevels(grade)
as.integer(gender)
as.integer(grade)

gender_char <- sample(c("female","male"),10000,replace=TRUE)
gender_fac <- as.factor(gender_char)
object.size(gender_char)
object.size(gender_fac)

as.character(gender)

is.character("red lorry,yellow lorry")
is.logical(TRUE)
is.list(list(a=1,b=4))
is.factor(gender)
is.factor(grade)

ls(pattern ="^is",baseenv())

is.numeric(2)
is.numeric(2L)
is.integer(2)
is.integer(2L)
is.double(2)
is.double(2L)

x <- "484.498498"
as(x,"numeric")
as.numeric(x)

y <- c(12,21,355,67)
as(y,"data,frame")
as.data.frame(y)

x <-"564.56454"
class(x) <- "numeric"
is.numeric(x)

y <- c(2,3,4,5,6,7,8)
for(i in y)
for (i in y) print(i)

num <- runif(50)
summary(num)

letters
letters[2:6]
LETTERS

fac <- factor(sample(letters[2:6],30,replace = TRUE))
summary(fac)

bool <- sample(c(TRUE,FALSE,NA),30,replace = TRUE)
summary(bool)

attributes(fac)

View(dfr)
new_dfr <- edit(dfr)
new_dfr <- fix(dfr)

peach <- 1
plum <- "fruity"
pear <- TRUE
ls()
ls(pattern="a")
ls.str()

browseEnv()

rm(peach,pear)
ls()

rm(plum)
ls()

#03回答
Q1:数字的三个内置类的名称是什么？
A1：浮点值numeric、整数integer和复数complex

Q2：用什么函数查找因子的水平值
A2：nlevels

Q3：如何把字符串“6.283185”转换为数字？
A3：使用as.character()函数

Q4：指出至少三个用于检视变量内容的函数
A4：is.character、is.list、is.factor

Q5:如何删除用户工作区中的所有变量？
A5：rm(list=ls())

#03练习1
#1）
class(Inf)
typeof(Inf)
mode(Inf)
Storagemode(Inf)
class(NA)
typeof(NA)
mode(NA)
Storagemode(NA)
class(NaN)
typeof(NaN)
mode(NaN)
Storagemode(NaN)

2）(pet <- factor(c("dog", "cat", "goldfish","hamster")))
pet <-sample(c("dog", "cat", "goldfish","hamster"),1000,replace = TRUE)
y <- c(1:10)
for (i in y)print(pet[[i]]) #达成了输出前十个任意动物的目的
as.integer(pet)#达成计数目的

3）tomato <- 1
potato <-2
bean <-3
ls(pattern = "a")
