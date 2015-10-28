# Notes-Processing

Notes of useful stuff for Processing.

## Table of Contents

* Functions

## Setup

Set Pixel Density According to Display Density

```
pixelDensity(displayDensity());
```

## Functions

You would be running this function repeatedly so the value eases towards its goal. For instance, inside the ```draw()``` function.

### Ease A Value

```
float ease(float value, float newValue) {
  float diff = value - newValue;
  
  if (abs(diff) > 0.01) {
    value -= diff/smoothing_factor;
  }  
  
  return value;
}
```