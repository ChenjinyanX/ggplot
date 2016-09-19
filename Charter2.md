## Key notes

### Every ggplot2 plot has three key components:
- **data**,
- A set of **aesthetic** mappings between variables in the data and visual properties, and
- At least one layer which describes how to render each observation. Layers are usually created with a **geom function**.

'''ggplot(mpg, aes(x = displ, y = hwy)) +geom_point() '''
- **Data**: mpg.
- **Aesthetic mapping**: engine size mapped to x position, fuel economy to y position.
- **Layer**: points.

### **data and aesthetic mappings** are supplied in **ggplot()**, then **layers** are added on with **+**

### the first two unnamed arguments to aes() will be mapped to x and y. 
This means that the following code is identical to the example above:
    '''ggplot(mpg, aes**(displ, hwy)**) + geom_point()'''

### Colour, size, shape and other aesthetic attributes
#### ggplot2 takes care of the details of converting data (e.g., ‘f’, ‘r’, ‘4’) into aesthetics (e.g., ‘red’, ‘yellow’, ‘green’) with a **scale**
- gives each point a unique colour corresponding to its class:aes(displ, hwy, colour = class)  
- aes(displ, hwy, shape = drv)
- aes(displ, hwy, size = cyl)
#### set an aesthetic to a fixed value, without scaling it
- the value “blue” is scaled to a pinkish colour, and a legend
is added:ggplot(mpg, aes(displ, hwy)) + geom_point(aes(colour = "blue"))
-  the points are given the R colour blue:ggplot(mpg, aes(displ, hwy)) + geom_point(colour = "blue")
#### colour and shape work well with categorical variables, while size works well for continuous variables
####  if there is a lot of data it can be hard to distinguish different groups. An alternative solution is to use facetting.

# leading the reader from ignorance to knowledge.
