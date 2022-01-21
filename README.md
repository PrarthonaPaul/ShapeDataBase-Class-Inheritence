# ShapeDataBase-Class-Inheritence

This program is a shape database that uses inheritence to create derived classes for rectangle, circle and triangle shapes from the base class called shape.

The user inputs the type of the shape followed by a name and its coordinates. 

# Examples:

<h3>Creating a Triangle: </h3>

triangle t1 1.0 1.0 2.0 2.0 3.0 3.0

where triangle is the shape type, t1 is the name of the shape and (1,1), (2,2), (3,3) are the three vertices of the shape. 

<h3>Creating a Circle: </h3>

For a circle, the user inputs the shape type, followed by the name, and the x and y coordinates of its centre and its radius. 

Example: circle c1 0.0 0.0 4.0

Here, c1 is a circle with a radius of 4 centred at the origin. 

<h3>Creating a Rectangle: </h3>

For a rectangle, the user inputs the keyword rectangle followed by the x and y coordinates of its centre and its height and width. 

Example: rectangle r1 0.0 0.0 4.0 6.0

here, the program creates a rectangle located at the origin with a width of 4 and a height of 6. 

# Other Commands and Error Checking 

Both the keywords and the names of the shapes are case sensitive. So, while r1 and R1 can refer two two different shapes, circle and Circle are not both valid commands. Some other keywords of the program are: 
area: it calculates the total area of all the shapes rounded to twp decimal points. 
    Example: 
              Input:   area 
              Output:  Total area = 74.2
draw: It lists all the shapes in the Database
    Example: 
              Input:  draw
              Output: triangle: t2 1.00 2.00 1.00 1.00 2.00 2.00 0.00 3.00 1.50 
                      triangle: t3 1.60 5.71 1.30 4.10 0.10 9.90 3.41 3.14 5.54 
                      triangle: t4 0.15 0.37 0.00 0.00 0.00 0.99 0.45 0.13 0.22 
                      
The program performs error checking to ensure that the keywords are valid and are spelled properly, none of the names of the shapes overlap with the keywoeks or the names of the shapes and that the correct number of data are entered by the user in the correct order.
If the error chack fails, the program outputs the appropriate error message. 


# Output Example

here is an example output of the program:

<pre>&gt; triangle t 1 1 2 2 3 3
created triangle
&gt; circle c1 1 8
Error: invalid input
&gt; circle c1 0 0 4
created circle
&gt; rectangle 5 5 5 5
Error: invalid input
&gt; rectangle r1 0 0 4 6
created rectangle
&gt; draw
triangle: t 2.00 2.00 1.00 1.00 2.00 2.00 3.00 3.00 0.00
circle: c1 0.00 0.00 4.00 50.27
rectangle: r1 0.00 0.00 4.00 6.00 24.00
&gt; area
Total area = 74.27
&gt; circle c1 0 0 2
Error: a shape with the name c1 already exists
&gt; 
</pre>
