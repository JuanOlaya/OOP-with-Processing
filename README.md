# Object-Oriented Programming (OOP) with Processing

This repository is associated with the courses: Object-Oriented Programming (OOP) and Computer Graphics, taught in the university [School of Arts and Letters](https://artesyletras.com.co/ingenieria-de-las-artes-digitales/) (Bogotá) by Juan Olaya since the semester 2016.2 to the present. 

For this course we use the Java library [Processing](https://processing.org/) and his JavaScript version [P5js](https://p5js.org/). The following are the components required for the course. 

## Table of contents
- [Class Car (One Instance + Move Right Method)](#1.-class-car:)
- [Class Car (Two Instances - Move right and left Methods)](#2.-class-car:)

#### 1. Class Car: 
One Instance + Move Right Method

<p align="center">
  <a>
    <img src="Images/Exercise1.gif" width=350 height=190>
  </a>
</p>

```
// Script that operates an instance of the class Car
Car car1;

void setup() 
{
  size(550,300);
  // Initialize Car object
  car1 = new Car();
}

void draw() 
{
  background(140);
  // Operate Car object.
  car1.move();
  car1.display();
}
```
```
class Car 
{
  color colour;
  float xpos;
  float ypos;
  float xspeed;
  
  Car() 
  {
    colour = color(#FE9601);
    xpos = width/2-100;
    ypos = height/2-40;
    xspeed = 3;
  }
  
  void display() 
  {
    // The car is just a square
    noStroke();
    fill(colour);
    rect(xpos, ypos, 100, 50);
  }
  
  void move() 
  {
    xpos = xpos + xspeed;
    if (xpos > width) 
    {
      xpos = -100;
    }
  }
}
```

#### 2. Class Car: 
Two Instances + Move Right/Left Methods

<p align="center">
  <a>
    <img src="Images/Exercise2.gif" width=350 height=190>
  </a>
</p>

#### 3. Class Car: 
Multiple Instances + ArrayList + Move Right/Left Methods

<p align="center">
  <a>
    <img src="Images/Exercise3.gif" width=350 height=190>
  </a>
</p>

#### 4. Class Car: 
Rebound Method + Multiple Constructors + Multiple Instances + ArrayList + Move Method

<p align="center">
  <a>
    <img src="Images/Exercise4.gif" width=350 height=190>
  </a>
</p>

#### 5. Class Car: 
Vectors for Movement + Rebound Method + Multiple Constructors + Multiple Instances + ArrayList

<p align="center">
  <a>
    <img src="Images/Exercise5.gif" width=350 height=190>
  </a>
</p>

#### 6. Class Ball: 
Vectors for Gravity + Rebound Method + + Multiple Instances + ArrayList

<p align="center">
  <a>
    <img src="Images/Exercise6.gif" width=350 height=190>
  </a>
</p>


#### 7. Coding Challenge 1: 
Multiple instances of the Class Car showing a X

<p align="center">
  <a>
    <img src="Images/CodingChallenge1.gif" width=350 height=190>
  </a>
</p>

#### 8. Coding Challenge 2: 
Multiple instances of the Class Node showing a network

<p align="center">
  <a>
    <img src="Images/CodingChallenge2.gif" width=350 height=190>
  </a>
</p>

### Processing Bibliography
- [Learning Processing - Second Edition - Shiffman (2015) Online version](http://learningprocessing.com/examples/)
- [Nature of Code - Shiffman (2012) Online version](http://natureofcode.com/book/)

***

# STUDENT SKETCHES
To see and interact with the sketches made by the students you can visit:
- [Object-Oriented Programming (2017.2)](https://www.openprocessing.org/class/56631/)
- [Computer Graphics (2017.2)](https://www.openprocessing.org/class/56656/)
- [Computer Graphics (2017.1)](https://www.openprocessing.org/class/56330/)
- [Computer Graphics (2016.2)](https://www.openprocessing.org/class/55669)

# EXAMPLE SKETCHES
To check the example sketches running please visit [OpenProcessing - Juan Olaya](https://www.openprocessing.org/user/65585/)

<p align="center">
  <a href="https://www.openprocessing.org/user/65585/" target="_blank">
    <img src="Images/openProcessingProfile.png" width=300 height=275>
  </a>
</p>

***

## Processing Links:
- [The Coding Train (Daniel Shiffman)](https://www.youtube.com/user/shiffman)
- [Hello Processing](http://hello.processing.org/)
- [OpenProcessing](https://www.openprocessing.org/)
- [Processing Foundation](https://processingfoundation.org/)
