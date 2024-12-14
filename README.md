# Matplotlib
Here, the code provided demonstrates various functionalities of Matplotlib for data visualization in Python. 
Here's a breakdown of each cell:

Cell 1 & 2:

Imports necessary libraries: matplotlib.pyplot (imported as plt) for plotting and numpy (imported as np) for numerical computations.
Creates an array x containing 150 evenly spaced values between 0 and 10 using np.linspace.
Calculates sine and cosine of x and stores them in y and z respectively.
Prints the content of x (optional for checking the generated data).
Cell 3:

Plots the sine wave (y) vs the x-axis (x) using plt.plot.
Displays the plot using plt.show.
Cell 4:

Similar to Cell 3, plots the sine wave but adds labels for x and y-axis using plt.xlabel and plt.ylabel. You can see an additional label "sine wave" unintentionally added, likely a typo.
Cell 5:

Creates a new array x with values between -10 and 10 using np.linspace.
Calculates the square of x and stores it in y.
Plots y vs x using plt.plot.
Displays the plot using plt.show.
Cells 6-9:

Demonstrate various line styles and markers available in Matplotlib.
Each cell plots y vs x with a different style defined by a string after the comma in plt.plot(x, y, 'style').
Here's a reference for some common styles:
'r+': Red color with plus markers
'm*': Magenta color with asterisk markers
'g--': Green color with dashed line
'b-': Blue color with solid line
'y:': Yellow color with dotted line
'k': Black color (default)
You can experiment with different styles and colors to customize your plots.
Cell 10:

Plots both sine (y) and cosine (z) waves on the same graph using separate plt.plot calls.
Uses dashed lines for both curves with green ('g--') for sine and red ('r--') for cosine.
Cell 11 & 12:

Creates a bar chart to represent course offerings and the number of students enrolled.
Defines course names (Coursesoffered) and student counts (values).
Creates a figure (fig) and adds an axes (ax) using fig.add_axes.
Plots bars using ax.bar(Coursesoffered, values).
Sets labels and title for the plot using plt.xlabel, plt.ylabel, and plt.title.
The second cell (Cell 12) unintentionally uses ax.bar again, likely meant to be ax.pie for a pie chart.
Cell 13:

Creates a pie chart to represent the same data as the bar chart.
Defines labels (languages) and colors (color) for the pie chart slices.
Uses ax.pie(people, labels=languages, colors=color) to create the pie chart.
Adds labels and title using plt.xlabel, plt.ylabel, and plt.title.
Notice the ax.bar(languages, people) line from Cell 12 is still present, likely a copy-paste error.
Cell 14:

Similar to Cell 13, creates a pie chart with an exploded slice to emphasize a specific category.
Defines myexplode as a list with one element set to 0.2 (20% outwards) for the first slice (English).
Uses ax.pie(people, labels=languages, colors=color, autopct='%1.2f%%', explode=myexplode) to create the pie chart with the explosion effect.
Cell 15:

Creates a larger pie chart with more exploded slices for better visualization.
Defines myexplode with multiple non-zero values to create different explosion percentages for each slice.
Uses ax.pie with explode set to myexplode to achieve the desired effect.
Cell 16:

Creates a scatter plot to show the relationship between two variables (x and y).
Uses `plt.scatter(x,
