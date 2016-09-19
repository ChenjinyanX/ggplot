## Key notes

### Every ggplot2 plot has three key components:
1. data,
2. A set of aesthetic mappings between variables in the data and visual properties, and
3. At least one layer which describes how to render each observation. Layers are usually created with a geom function.

 ''' ### ggplot(mpg, aes(x = displ, y = hwy)) +geom_point()'''
1. Data: mpg.
2. Aesthetic mapping: engine size mapped to x position, fuel economy to y
position.
3. Layer: points.
