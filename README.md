Download Link: https://assignmentchef.com/product/solved-comp1210-activity6-conditionals-and-loops-ii
<br>
By the end of this activity you should be able to do the following:

<ul>

 <li>Understand the basics of the ternery <em>conditional operator</em></li>

 <li>Understand the basics of the <em>for loop</em>, <em>for each loop</em>, and the <em>do-while loop</em> Ø Understand the basics of the <em>switch</em> statement</li>

</ul>

<strong>Description: </strong>

In this activity you will create two classes. Temperatures will hold a set of integer values representing daily temperatures. TemperatureInfo will allow users to interact with the Temperatures class.<strong> </strong>

<strong>Directions: </strong>

<u>Don’t forget to add your Javadoc comments for your classes, constructor, and methods in this activity</u>.

<strong>Part 1: Temperatures: instance variable, method stubs  </strong>

<ul>

 <li>Create a class called Temperatures, which will hold a set of integer values representing daily temperatures.</li>

 <li>Add an instance variable with the name <em>temperatures</em> to your class that is of type ArrayList with generic type Integer.</li>

 <li>Add method stubs for the following methods<strong>. </strong></li>

</ul>

o The constructor takes an ArrayList of integer values

!!! o getLowTemp: takes no parameters; returns an integer value o getHighTemp: takes no parameters; returns an integer value o lowerMinimum: takes an int parameter; returns an integer value o higherMaximum: takes an int parameter; returns an integer value o toString: no parameters; returns a String

<strong>Part 2: Temperatures: constructor, getLowTemp  </strong>

<ul>

 <li>In your constructor, set <em>temperatures</em> equal to <em>temperaturesIn</em>.</li>

 <li>In getLowTemp, first return 0 if the ArrayList is empty:</li>

 <li>Now iterate through the entire list and find the lowest temperature:</li>

</ul>

Finally, after the loop, return the lowest temperature:

<strong>Part 3: getHighTemp  </strong>

<ul>

 <li>In getHighTemp, again return 0 if there are no temperatures in the ArrayList:</li>

 <li>This time, use a <em>for each</em> loop to iterate through the list of temperatures to find the highest temperature.</li>

 <li>Add code to the toString method to return a string containing the low and high temperatures (hint: make a method call to getLowTemp and getHighTemp):</li>

</ul>

<strong>Part 4: lowerMinimum &amp; higherMaximum  </strong>

<ul>

 <li>The lowerMinimum method takes an int value and returns the parameter if it is lower than the value returned by getLowTemp. Otherwise, it returns the return of getLowTemp.</li>

 <li>The higherMaximum method takes an int value and returns the parameter if it is greater than than the value returned by getHighTemp. Otherwise, it returns the return of getHighTemp.</li>

 <li>Test your methods in the interactions pane:</li>

</ul>

Note that you should <u>not</u> use the generic &lt;Integer&gt; when declaring the ArrayList in interactions.

Ï¼ÏÏimport java.util.ArrayList;

Ï¼ÏÏArrayList tempList = new ArrayList();

Ï¼ÏÏtempList.add(34);

Ï¼ÏÏtempList.add(52);

Ï¼ÏÏtempList.add(36);

Ï¼ÏÏtempList.add(65);

Ï¼ÏÏTemperatures temps = new Temperatures(tempList);

Ï¼ÏÏtemps.getLowTemp() ÏÏÏÏ34

Ï¼ÏÏtemps.getHighTemp() ÏÏÏÏ65

Ï¼ÏÏtemps.lowerMinimum(33) ÏÏÏÏ33

Ï¼ÏÏtemps.lowerMinimum(35) ÏÏÏÏ34

Ï¼ÏÏtemps.higherMaximum(64) ÏÏÏÏ65

Ï¼ÏÏtemps.higherMaximum(67)

<h1>ÏÏÏÏ67</h1>







<strong>Part 5: TemperatureInfo </strong>

<u>Don’t forget to add your Javadoc comments; the class and main method will need one</u>.

<ul>

 <li>Download the <u>canvas file</u> for this activity and save it in same folder as the classes for this activity. After you have created and compiled part or all the <em>main</em> method described below, use the canvas file in conjunction with debugger and/or run the program in canvas mode.</li>

 <li>Create a class called TemperatureInfo with a main method. <u>Declare and instantiate a Scanner</u> <u>object called userInput that reads from System.in</u>.  <u>Declare and instantiate an ArrayList with</u> <u>generic type Integer called tempsList</u>.  Remember to import the Scanner and ArrayList classes.</li>

 <li>Create the following <em>do while</em> loop that will read in temperature values, one per line, and add each to tempsList until the user presses enter with no value to indicate that there are no more temperatures to be input. After all of the temperatures have been read in and added to tempsList, create a Temperatures object with the tempsList:</li>

</ul>




<ul>

 <li>Create a menu by using a <em>do while</em> loop that contains a <em>switch</em> statement to select among user choices for the following: [L]ow temp, [H]igh temp, [P]rint, [E]nd</li>

</ul>

where ‘L’ prints the low temperature, ‘H’ prints the high temperature, ‘P’ prints the Temperatures object temps, ‘E’ ends the the program (i.e., ends the <em>do while</em> loop).







Run your program as below to test its output:

MM«M —-jGRASP exec: java TemperatureInfo

¼¼§MEnter a temperature (or nothing to end list): 34

¼¼§MEnter a temperature (or nothing to end list): 56

¼¼§MEnter a temperature (or nothing to end list): 78

¼¼§MEnter a temperature (or nothing to end list): -10 ¼¼§MEnter a temperature (or nothing to end list): 95

¼¼§MEnter a temperature (or nothing to end list):

¼¼§MEnter choice – [L]ow temp, [H]igh temp, [P]rint, [E]nd: L MM§M   Low is -10

¼¼§MEnter choice – [L]ow temp, [H]igh temp, [P]rint, [E]nd: H MM§M   High is 95

¼¼§MEnter choice – [L]ow temp, [H]igh temp, [P]rint, [E]nd: P

MM§M   Temperatures: [34, 56, 78, -10, 95]

MM§M   Low: -10

MM§M   High: 95

¼¼§MEnter choice – [L]ow temp, [H]igh temp, [P]rint, [E]nd: E MM§M   Done MM§M MM©M —-jGRASP: operation complete.







<ul>

 <li>Run your program in Canvas mode using the canvas file you downloaded. Be sure to wait for the program to ask for input before keying in the temperature and pressing ENTER.  Remember that you can control the speed with the delay slider in canvas window or debug tab.</li>

 <li>Finally, submit your .java files to Web-CAT.</li>

</ul>