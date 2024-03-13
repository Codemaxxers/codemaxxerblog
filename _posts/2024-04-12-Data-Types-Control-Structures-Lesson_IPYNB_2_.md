---
toc: True
comments: True
layout: post
title: Data Types and Control Structures Lesson
type: hacks
courses: {'csse': {'week': 1}, 'csp': {'week': 1, 'categories': ['4.A']}, 'csa': {'week': 0}, 'labnotebook': {'week': 3}}
---

# Data Types and Control Structures Lesson 
*By Luna and Tanisha and Rachit* 

Find link to notebook in Slack coding channel and follow along. WGET to have easy access to these materials (WGET not required for the lesson itself)

# Data Types

## Primitive Data Type Overview
- In Java there are eight primitive types : int, byte, short, long, float, double, boolean, and char
- These data types are NOT considered objects, they represent just values. 
- Ex. int x = 20; x stores the value of 20
- Stored on the stack memory


![datatype_table](https://github.com/lightkurve/lightkurve/assets/111611921/415762a8-99aa-43d7-80eb-62ee92f2168a)


## Reference Data Type Overview 
- A variable of a class type is a reference data type
- Created by the programmer not defined by the Java language 
- Contains the reference of a dynamically created object 
- Ex.  Person p = new Person () . p will reference the address of the person object. 
- Stored on the heap memory 


## 3 Main Differences Between Primitive and Reference Types

### 1. ASSIGNMENT

**Primitive**:  When we assign a value to primitive data types, the primitive VALUE is copied. : 


```Java
// Changing the value of b, WILL NOT change the value of a

Int a = 50 
Int b = a

```

**Reference**:  When we assign value to reference type the address is copied. When we assign reference type values, both will point to the same address. The object will be shared between two represent variables. 


```Java
// Changing anything of f, WILL change p

Person p = new Person(“sample_name”); 
Person f = p; 

```

### 2. COMPARISON

**Primitive**: When we compare primitive variables (==) , their values will be compared 


**Reference**: When we compare reference variables (equals() method) , their addresses will be compared. Two objects with the same exact content may not be seen as not equal. 



```Java
public class Comparison {
    public static void main(String[] args) {
        // Primitive 
        int a = 20; 
        int b = 20; 

        // Reference
        String str1 = new String("word");
        String str2 = new String("word");

        // Compare Primitive with (==) : Primitive types are compared by VALUE
        if (a==b) {
            System.out.println("Value of a equals value of b"); 
        } else {
            System.out.println("Value of a DOES NOT equal value of b");
        }

        // Compare Reference with (==) VS .equals() : Reference types are compared by REFERENCE not value

        if(str1 == str2){
            System.out.println("Str1 and Str 2 have the same content (==)");
        }
        if(str1.equals(str2)){
            System.out.println("Str1 and Str2 have the same content (equals) ");
        }

    }
}

Comparison.main(null);

```

    Value of a equals value of b
    Str1 and Str2 have the same content (equals) 


### 3. NULL VALUES 

**Primitive**: Primitive types can never be null. No assignment will result in their default value (see table in primitive data section) 

**Reference**: Reference types can be null. Null signified the absence of an assigned value. 





## Extra  
### Visualizing Stack Memory Vs Heap Memory 
<img width="518" alt="image" src="https://github.com/lightkurve/lightkurve/assets/111611921/f9b58a26-8c1b-4e45-9705-2bf14e6033fa">


### Resources
- College Board Videos are great resources. For further clarification watch: [1.2.1 and 1.2.2](https://apclassroom.collegeboard.org/8/home?apd=auzlevozkr&unit=1)
- This [video](https://youtu.be/n9S2Ig0S3AY) is also a great resource

## Hacks

1. Create a class on a topic of your choosing where in the main function you assign some values to those integers. Then, create a comparison statement with each type of comparison. Make it have a purpose, add a scenario.
2. Draw a diagram for it

# Methods and Control Structures


```Java

```
