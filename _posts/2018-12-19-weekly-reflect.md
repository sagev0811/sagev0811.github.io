---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of _Dominican Republic_ by _Sage Vega_

## Describe your program



In this program, I designed the flag for the Dominican Republic. I expect to get at least a 2 on this project.


## Current output



* * *
![Flag](/images/flag.png)
* * *

## Describe your process.


I made a size function to equal 100, representing the size of the rectangle. The width and height functions are to represent the proprtions of the flag, which is 2:3. They are multiplied by 100, which is the size function, to make it bigger, as it would be too small if it's just 2 and 3. Then, I made rectangle functions for the different rectangles of the flag. After that, I made different place-image functions (BR1,RR1,RR2,BR2) to put the blue and red rectangles in the correct places using the right coordinates, on the white rectangle, which is the background of the flag. I had to make those different function names as just using the place-image function alone would place the rectangles onto seperate white rectangles. It allowed me to place the rectangles on the same white rectangle. 

​



## Explain your code.
As I said earlier, size is to represent the size of the rectangle. The width and height functions are to represent the proprtions of the flag, which is 2:3. They are multiplied by 100, which is the size function, to make it bigger, as it would be too small if it's just 2 and 3. BR is for the blue rectangles, RR is for the red rectangles, and WR is for the white rectangle, making the background, like I mentioned earlier. The width and height of the white rectangle is multiplied by 2 because it makes it able to contain all the rectangles on it. "Solid" makes the shape solid and colored in, unlike "outline" which would just make it an outline of a rectangle. 


* * *

```
size = 100
width = size * 3
height = size * 2
BR = rectangle(width,height,"solid","blue")
RR = rectangle(width,height,"solid","red")
WR = rectangle(width * 2,height * 2,"solid","white")
```

* * *





## Program code

```
include image
size = 100
width = size * 3
height = size * 2
BR = rectangle(width,height,"solid","blue")
RR = rectangle(width,height,"solid","red")
WR = rectangle(width * 2,height * 2,"solid","white")
BR1 = place-image(BR,size,50,WR)
RR1 = place-image(RR,500,50,BR1)
RR2 = place-image(RR,size,350,RR1)
BR2 = place-image(BR,500,350,RR2)
flag = BR2
```
