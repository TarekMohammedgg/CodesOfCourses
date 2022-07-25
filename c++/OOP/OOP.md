- 
- what is Oop ?↔the oop is the way or method to create a software system
- what is objects ?↔is the any thing can create like students or products (Tingable - Intingable)
- what is classes?↔is the stand object or blueprint you put the standard attributes and function of your objects
- what is the Access Modifires?↔it is the methode that you can access to the data .. And it divid to 2 type (private - public )
- what is the private access (data hiding )  ?↔it is the way that not any can access to it and you must create like bridge or method to apply any one to access to it .
- How to create class?↔Like creating struct ..
- what is the setter or mutator ?↔it is the methode that you can modify or change on the attributes of the objects
- what is the accssor or getter ?↔it is the methode that you make to call the attributes or operations
- How you create the class files ?↔you can separating class into 2 files  : 1.header ->.h 2.implementation files ->.cpp 3. it is the client code(in this case main function) ..
    - what is initialization list↔it is a method to initialize variables in [Constructors](../Constructors.md)..
        - 
- 
- what is the function of [Destructors](../Destructors.md)↔it will be called automatically after end the object .. 
- [Constructors](../Constructors.md)^^ and method overloadin^^ 
    - هي عبارة عن استخدام نفس اسم الfunction و لكن الاختلاف بيكون في ال signature or parameter 
    - ![](local://C:/Users/tarek/remnote/remnote-629634e757d3b4003536f33e/files/NZDY-L9C3YSaViwQcVkYpeD3rtXFp4jniewfz6Ms0Ig3YIntdkEWlKTYboclw0St8gXDMwOYg26u97rDeZGPcKjCtTTUM-G1KPx61iVOrHhvbfUZcmXk1gF0eu0_-7jq.png) 
- The default copy constructors 
    - يعني انك ممكن تأخد نسخة من object انت عملته قبل كده 
    - مثال : 
    - ```cpp
Distance d1 (12 ,5.5) ; //Distance (int feet , float inches  ) 
Distance d2 (d1) or Distance d2 =d1 ;
d2.getdis() ; //void getdis (){cout<<"feet =" <<feet<<"\t"<<"inches =" <<inches<<endl ; 
// The output: 
feet =  12    inches = 5.5 

```
- Passing Objects To Methods 
    - يعني انك تخلي ال object كأنه argument في object تاني 
    - ```cpp
 class Distance 
 void adddis (Distance d1 , Distance d2) ; //Distance.h 
 void adddis(Distance d1 , Distance d2 ) {
 feet = d1.feet + d2.feet ; 
 inches = d1.inches + d2.inches ; 
 }// Distance.cpp 
 // ------IN Main--------
 Distance d1(11. 3.5) ; 
 Distance d2(12 ,1.5 ) ; 
 d1.adddis (d1 , d2 ) ; 
 d1.getdis() ; 
 the OUtput 
 feet = 22    inches = 5 
  
 
```
- Static members  
- Operator Overloading 
- Inheritance 
- Inheritance Function Overriding 
- Multiple Inheritance
- Polymorphism and Virtual Functions 
- Abstract Class and Final Class
- 
- 
- 
