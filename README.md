# Notes-Processing

Notes of useful stuff for Processing.

## Table of Contents

* Setup
* Functions
* Libraries

## Libraries

* Syphon. Create a video feed from a PGraphics.

## Setup

Set Pixel Density According to Display Density

```java
pixelDensity(displayDensity());
```

## Functions

You would be running this function repeatedly so the value eases towards its goal. For instance, inside the ```draw()``` function.

### Ease A Value

```java
float ease(float value, float newValue) {
  float diff = value - newValue;
  
  if (abs(diff) > 0.01) {
    value -= diff/smoothing_factor;
  }  
  
  return value;
}
```

### Is Even

```java
boolean isEven(int n){
  return n % 2 == 0;
}
```

### Timestamp

A timestamp formatted in `yymmdd_hhmmss`.

```java
String timestamp = (year() + "").substring(2,4) + nf(month(), 2) + nf(day(), 2) + "_" + hour() + minute() + second();
```
