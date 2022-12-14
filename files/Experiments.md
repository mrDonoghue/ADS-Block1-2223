# Sorting Experiments

## Bare minimum experiment for comparing algorithms:
* test each algorithm on a range of input sizes that spans several orders of magnitude (the longest input size should take *at least* 10 seconds for the slower of the algorithms)
* Compare the algorithms across all of these input sizes, often easiest with a plot
* Note that later in this file, **I provide code for generating plots** given files with data
## General plan for generating data
* make a function/method that conducts the whole experiment for a single algorithm when given:
  - a list/array of the input sizes
  - the function/method to time
  - where to record the data
* this experiment function/method will need to iterate through the array/list of sizes and:
  - make a random array of the right size
  - start a "stopwatch"
  - run the given sorting function/method
  - immediately stop the "stopwatch"
  - record this datapoint as "SIZE TIME" (replacing SIZE and TIME with the actual numbers) in a file
* this plan involves using a function/method as an argument to a function/method. Since you've probably never done this, I'm providing an example/skeleton to build off of: See [this file for the Java version](JavaTestingExample.md)  or [this file for the Python version](PythonTestingExample.md)


## Plotting
Open the [SortingPlotting](https://replit.com/team/Algos-Block1-2223/SortingPlotting) repl
# How to use my plotting code
* Create a file for each plotline you want in the plot
  * the name of the file before the extension will be used as the label in the legend of the plot
  * the file should have a series of text lines where each line of the file corresponds to a single data-point for a single sorting algorithm
  * each line of the file should be two numbers separated by a space
  * the first number should be the array size
  * the second number should be the time it took to sort
* Once your SortingPlotting repl contains all of the files you want, hit the run button
  * In the console, enter each filename followed by enter/return
  * After the last filename, hit enter/return twice in a row, to let my program know that you're done
  * My program should show you a plot
  * Look for the save button in the plot window to save the image to your repl.

## Analysis
#### Record your answers to the following in a file in your [SortingPlotting](https://replit.com/team/Algos-Block1-2223/SortingPlotting) repl
# How to use my plotting code
* What is the biggest conclusion we can draw from the experiments?
* Based on the shape of the graphs, which 3 sorts have (big picture) the same long-term running time?
* what simple function has approximately that shape?
* Which sort(s) are a stand out as much much much better?
* Plot just the fast sort(s) so you can get a better sense of the shape of their graphs
* What simple function does this shape look like?