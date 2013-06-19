
README for StackTagGraphs
-------

StackExchangeTagGraphs by Owen Mundy owenmundy.com



Description
-------

Visualize tags from Stack Overflow and other Stack Exchange websites as network graphs.



Usage
-------

Step 0: inc/config.php.example

 1. Rename inc/config.php.example to inc/config.php
 2. Using the "create table syntax" in config.php, create the database and MySQL tables
 3. Define database connection information and StackExchange site and table names
 4. Uncomment and enter apikey to raise daily limits

Step 1: import.php

 1. Run import.php which
 * Exports question data from the Stack Exchange API http://api.stackexchange.com 
 * Finds tag relationships in question data
 * Saves this data in MySQL

Step 2: export.php

1. Run export.php which
2. Selects data from database
3. Creates and formats Python code to be copied/pasted into NodeBox

Step 3: Select colors

 1. Use _____ to export colors
 2. Use PaletteVisualizer http://owenmundy.com/work/PaletteVisualizer/ to edit colors you wish to use
 3. Alter palette dict to contain colors to suite the site you are working with

Step 4: nodebox.py

 * Copy/paste Python code from export.php into nodebox.py and open in NodeBox 1.9.7x
 * Run the code
 * Export a PDF or PNG file



References
-------

StackExchange API Documentation http://api.stackexchange.com/docs



Notes
-------

Each data set/graph may take a lot of tweaking and many different renders to generat satisfactory results
