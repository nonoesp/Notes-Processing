# Notes-Processing

Notes of useful stuff for Processing.

## Table of Contents

* Functions

## Functions

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