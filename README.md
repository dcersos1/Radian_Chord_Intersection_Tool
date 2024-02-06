# Radian Chord Intersection Tool 

Dan Cersosimo | Developer

**Contextualization**

This tool harnesses an algorithm I designed to calculate the number of distinct intersections between chords in a circle given the radian measures of their respective start and end points along a circle. Essentially, I implemented user interactive features that allow for said user to make use of this tool in accordance with their chord data. 

**Overview:**

The program is broken down into 3 core functions which work off of each other's outputs as inputs for the subsequent one. The Retrieve_Chord_Data() function is initially called and welcomes the user to the tool. Following this, the function progresses with questions asking for the number of chords they would like in the circle. Following this, they are asked to provide input for the start and end points for each chord. The Retrieve_Chord_Data() function processes this data into a dictionary housing the start and end points for each chord to be interpreted by the Construct_Circle() function. This function builds a circle and utilizes the organized chord data to visualize the chords on the circle while calculating and returning the slope and intercept for each chord in a dictionary. Subsequently, the Intersections() function utilizes the slope and intercept data to iterate through each combination of chords to evaluate a system of equations and find distinct intersection points. The logic of this function ensures the intersections are within one radius (1) from the center (0,0) to count as valid. Following this, it returns the intersections between chords, their respective cartesian coordinates within the circle, and a total count of unique intersections.

**How to Run:**

This was executed in a Jupyter Notebook and saved as a .ipynb file. As a result, running a Jupyter Notebook file is needed. In addition, matplotlib.pyplot and numpy must be installed and accessible.

**Big-O Runtime:**

One of the functions exhibits a nested loop and therefore the big-O runtime would be O(n^2). 

**Documentation:**

Specifics regarding the logic of the code are detailed in comments within the file itself.



*Feel free to experiment with your own input and I hope you enjoy this program!*
