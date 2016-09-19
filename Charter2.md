## Key notes

### Every ggplot2 plot has three key components:
- **data**,
- A set of **aesthetic** mappings between variables in the data and visual properties, and
- At least one layer which describes how to render each observation. Layers are usually created with a **geom function**.

 ### ggplot(mpg, aes(x = displ, y = hwy)) +geom_point() 
- **Data**: mpg.
- **Aesthetic mapping**: engine size mapped to x position, fuel economy to y position.
- **Layer**: points.

### **data and aesthetic mappings** are supplied in **ggplot()**, then **layers** are added on with **+**

### the first two unnamed arguments to aes() will be mapped to x and y. 
This means that the following code is identical to the example above:
'''ggplot(mpg, aes**(displ, hwy)**) + geom_point()'''

### Colour, size, shape and other aesthetic attributes
- aes(displ, hwy, colour = class)
- aes(displ, hwy, shape = drv)
- aes(displ, hwy, size = cyl)
