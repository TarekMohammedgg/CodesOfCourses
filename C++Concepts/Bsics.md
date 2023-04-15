

## why you like to learning c++ ??

because i want to learn about programming , it is my job and i want to be a great in this field . 

------------

### The concepts in this course : 

1. introduction to c++ . 
2. what is source code , object code , compiler , algorithm ? 
3. introduction to  variables .
3. (complete course in c++) -> how to  learn the max integer can understand in int or any data type
3. (complete course in c++) ->functions (default &overloading & call by reference & polymorphism& lamda & pointer ). 
3. (complete course in c++) ->oop -> (class - constructors- deconstructors - operation overloading  ) .
3. (complete course in c++) ->oop -> (templates  & namespace & linked list   ) . 

----------------------------


### 1.introduction to c++ . 

### what is c++ ? 

#### c++ is used in general purpose : 

- create all types of programs : games , operating systems , browser , compilers , embedded systems , all others general purpose software . 

#### compiled  :

- converting code that you understand into code that your computer understands .
- building code . 
- compile-time errors . 

#### case sensitive : 

- c++ distinguishes between upper case and lower case letters . 
- my variable != My Variable . 

## why c++ was created ? 

- because it is understandable and easy to use fast execution of demanding tasks . 

------------

## 2.what is source code , object code , compiler , algorithm ? 

- source code =compiler=> machine code . 

### source code: 

- is the base code or the simple form from code and it can be able pseudocode or c++ code . 

### object code : 

- usually is form of ones or zeros  , the computers can understand it . 

### algorithms : 

- algorithms is list of ingredients and steps that the computer needs to do your orders . 

-------

## 3.introduction to  variables : 

- you can get rid the junk text in your command by 

```c++
system("pause>0") ; 
```

------

## complete course c++: 

### to learn the max integer can understand in int or any data type   

```c++
in generall => -2^(n-1) and 2^(n-1)-1 
 int => -2^(32-1) and 2^(32-1)-1 
  if the data type is unsigned => 2^(32)-1 
      32-1 عشان فيه واحد بت للاشاره 
      
      
```

```c++
wchar_t x = 't' ; == char x = 't'  ;
but the different is the wchar take much memory to save the character 
```

```c++
auto result = a + b+ c ; 
// must on the same line 
typeid(YourVariable).name() => to know the datatype of your variable .. 
decltype(yourvariableYouWant) variableName = value => if you want to declare variable be the same type of another variable .. 
```

```
0xhexnumber or 0bbinar
std::hex => to print hex number .
```

```c++
to create ptr in dynamic memory : int * dnumber = new int[1] ;
but you must delete the variable by use delete dnumber or if is array delete[] arrayname
```

![](E:\study.githube\imgs\c++completecourse.png)

![](E:\study.githube\imgs\dynamic memory png.png)

## function 

```c++
// function overloading 
double sum (double a , double b ) {
    double res = a+b ; 
    return res; 
}
double sum (double a , double b , double c) {
    double res = a+b+c; 
    return res; 
}
// polymorphism : the same name but the argument not same and return value also . 
double sum (double a , double b ) {
    double res = a+b ; 
    return res; 
}
int  sum (int a , int b ) {
    int  res = a+b; 
    return res; 
}
// lambda function method 
// if you want send it all by refrence type [&] or one refrence and b value type [a , &b] 
auto sum = [your capture ] (int a , int b )->int {
   int res ; 
    res = a + b ; 
    return res ; 
}
// function pointer 
int (*sum) (int , int ) ; 

```

![](G:\Shared drives\MyDrive\Files\study.githube\imgs\TheFunctions.png)

```c++
#include<iostream>
#include<math.h>
using namespace std ;
// default function
int sum (int a , int b ) {
int res ;
res = a + b ;
cout<<"the sum is : " << res << endl ;
return 0 ;}
// by reference
int sub (int *a , int* b ){
int res = *a - *b ;
cout<<"the sub is:" << res << endl ;
a = a+ 10 ;
b = b+ 10 ;
return 0; }
// overloading
int sum (int a , int b , int c  ) {
int res ;
res = a + b + c  ;
cout<<"the sum is : " << res << endl ;
return 0 ;}
// polymorphism
double sum (double a , double b ) {
double res ;
res = a + b ;
cout<<"the sum is : " << res << endl ;
return 0 ;}
// lamda
 auto  multi = [=] ( long  a ,  long  b)-> long {
 long res = a * b ;
 cout<<"the multiplication is : " << res<<endl ;
return 0 ;
 } ;
int main(){
int a , b ;
a = 10 ;
b = 11 ;
int c = 12 ;
int res1= sum(a , b ) ;
int res2 = sub(&a, &b ) ;
cout<<"the new a : " << a << "\tthe new b : " << b << endl ;
int res3  = sum(a , b ,c ) ;
double res4 = sum(10.5 , 12.5 ) ;
long  res5 = multi(a , b ) ;
return 0 ; }

```

```c++
// function pointer work with lambda method very well .. 
// function pointer is use to point to another function ..and it should point to the same signature  
int sum (int a , int b) {
    int res ; 
    res = a+b ; 
    return res ; 
}
int (*sumptr)(int , int ); 
int main(){
    sumptr = &sum ; // must be insert main function .. 
    int rs = sumptr(10 , 9 ) ; 
    cout<<rs<<endl ;
    
    
    return 0; 
}
```

### function pointer 

<img src="E:\study.githube\imgs\FunctionPointer.png" style="zoom: 80%;" />

<img src="E:\study.githube\imgs\functionpointerwithlamda.png" style="zoom: 80%;" />

## oop 

### fundamental about class  

![](E:\study.githube\imgs\fundementalaboutoop.png)

## constructors & deconstructors 

```c++
//header
class rectangle {
    public  :
    int width , height ; 
    rectangle (int w , int h ); 
    int area(); 
    ~rectangle(); 
};
//implementation 
int rectangle :: area(){
    int res = this -> width * this->height ; 
    return res; 
}
rectangle :: rectangle (int w , int h ){
    this->width = w; 
    this->height = h ; 
    
}
rectangle ::~rectangle (){
    cout<<"Thank you" <<endl ;
}
```

### operator overloading 

```c++
#ifndef RECTANGLE_H
#define RECTANGLE_H

class rectangle {
    public  :
    rectangle (int w , int h );
    int area();
    ~rectangle();
    rectangle operator + (rectangle &rect ) ;
    private:
            int width , height ;

};

#endif // RECTANGLE_H

```

```c++
#include "rectangle.h"
#include<iostream>
using namespace std;
//implementation
int rectangle :: area(){
    int res = this -> width * this->height ;
    return res;
}
rectangle :: rectangle (int w , int h ){
    this->width = w;
    this->height = h ;

}
rectangle ::~rectangle (){
    cout<<"Thank you" <<endl ;
}
rectangle rectangle:: operator + (rectangle &rect ) {
int width = this->width + rect.width ;
int height = this->height + rect.height;
cout<<"the width is : " << width << endl ;
cout<<"the height is : " << height << endl;
return rectangle (width , height ) ;  }


```

### templates 

```c++

```

### instance 

```c++ 
if class is protected you can inheriet any information from father to brother , but you can not call it from main function (instance ) . 
```

### virtual 

```
virtual : if you want to make overriding on any function and you must put implementation =0 in father class 
```

