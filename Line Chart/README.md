<h1 id="bkmrk-line-graph"><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>Line Graph</strong></span></h1>
<p id="bkmrk-%C2%A0"></p>
<ul id="bkmrk-a-line-graph%2C-also-k">
<li class="null" style="text-align: justify;">A Line Graph is a type of data visualization that displays how various data points change over time.</li>
<li class="null" style="text-align: justify;">Uses points connected by line segments from left to right to demonstrate changes in value.</li>
<li class="null" style="text-align: justify;">Monitor the behavior in a set of data.</li>
</ul>
<p id="bkmrk-%C2%A0-1"></p>
<h2 id="bkmrk-purpose"><span style="text-decoration: underline;"><strong>Purpose</strong></span></h2>
<ul id="bkmrk-the-graph%E2%80%99s-main-pur">
<li class="null" style="text-align: justify;">To monitor and compare the levels of students in math and science tests for a few selected months.</li>
<li class="null" style="text-align: justify;">The graph's two lines, one for each subject (Math &amp; Science), which make it easy to compare and evaluate the subjects performance over months.</li>
</ul>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-requirements"><span style="text-decoration: underline;"><strong>Requirements</strong></span></h2>
<ul id="bkmrk-height-and-width--%C2%A0">
<li class="null" style="text-align: justify;"><strong>Height and Width -&nbsp;</strong>The heights and widths are used to adjust the size of the graph layout. You can specify the height and width in centimeters (cm), millimeters (mm), or points (pt).</li>
<li class="null" style="text-align: justify;"><strong>Y axis max and max values - </strong>Define the minimum and maximum values of the y-axis. They are used to set the range of the axis for plotting graphs.</li>
<li class="null" style="text-align: justify;"><strong>X and Y tick labels - </strong>Controls the labels displayed on the x and y-axis ticks.</li>
<li class="null" style="text-align: justify;"><strong>X and Y axis labels - </strong>Providing a description or naming the axes of a graph or plot.</li>
<li class="null" style="text-align: justify;"><strong>Legends -&nbsp;</strong>To provide the descriptive names for the plots or a group of plots.</li>
<li class="null" style="text-align: justify;"><strong>Title -&nbsp;</strong>To provide the name for the graph.</li>
<li class="null" style="text-align: justify;"><strong>Color of the lines </strong>- The color should be customizable based on the subject.</li>
<li class="null" style="text-align: justify;"><strong>Shift Values - </strong>If the two data points overlap with each other, then shift each label on any directions.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-when-two-points-ahs-">
<li class="null" style="text-align: justify;">When two data points have the same value, they overlap with each other.</li>
<li class="null" style="text-align: justify;">The graph layout overflows in the page layout when we feed too much data.</li>
<li class="null" style="text-align: justify;">Adjusting the tick label when it has its full name.</li>
</ul>
<p id="bkmrk-%C2%A0-4"></p>
<h2 id="bkmrk-"></h2>
<h2 id="bkmrk-latex-link"><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h2>
<h5 id="bkmrk-lapis-reports---%3E%C2%A0" style="padding-left: 40px;">LaPIS Reports --&gt; Charts --&gt; Line Chart.tex</h5>
<p id="bkmrk-%C2%A0-5"></p>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-define-variables%3A-de" data-sourcepos="25:1-66:0">
<li data-sourcepos="25:1-29:0">
<p style="text-align: justify;" data-sourcepos="25:4-25:24"><strong>Define Variables:</strong></p>
<ul style="text-align: justify;" data-sourcepos="26:5-29:0">
<li data-sourcepos="28:5-29:0">Declare <em>\coords</em> with<em> \newtoks</em> command globally for tokenizing the coordinate values. [line no. 12]</li>
<li data-sourcepos="26:5-26:77">Calculate<em> graphHeight</em> and<em> graphWidth</em>&nbsp;based on the input dimensions.</li>
<li data-sourcepos="27:5-27:61">Set <em>ymin </em>and <em>ymax</em> based on the input Y-axis limits.</li>
<li data-sourcepos="28:5-29:0">Define custom colors for the lines (e.g., rgbColor1, rgbColor2).</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="30:1-32:0">
<p data-sourcepos="30:4-30:30"><strong>Begin TikZ Environment:</strong></p>
<ul data-sourcepos="31:5-32:0">
<li data-sourcepos="31:5-32:0">Initiate the TikZ picture environment for creating the graph.</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="33:1-42:0">
<p data-sourcepos="33:4-33:19"><strong>Create Axis:&nbsp;</strong></p>
<ul data-sourcepos="34:5-42:0">
<li style="text-align: justify;" data-sourcepos="34:5-34:127">Define the axis properties, including title, height, width, X and Y-axis limits, tick labels, and labels for the X and Y-axes.</li>
<li style="text-align: justify;" data-sourcepos="35:5-35:64">Enable major grids for both axes with a dashed line style.</li>
<li style="text-align: justify;" data-sourcepos="36:5-36:74">Set the major X-tick style to transparent to avoid cluttering the graph.</li>
<li style="text-align: justify;" data-sourcepos="37:5-37:87">Enable placing data point values near corresponding coordinates with a black color.</li>
<li style="text-align: justify;" data-sourcepos="38:5-38:61">Set axis lines to be drawn on the bottom and left sides.</li>
<li style="text-align: justify;" data-sourcepos="39:5-39:39">Set the axis line color to white.</li>
<li style="text-align: justify;" data-sourcepos="40:5-40:68">Slightly enlarge the Y and X-axis limits for better visualization.</li>
<li style="text-align: justify;" data-sourcepos="41:5-42:0">Rotate the X-axis tick labels by 45 degrees for better readability when there are many labels.</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="43:1-57:0">
<p data-sourcepos="43:4-43:26"><strong>Loop through the lines:&nbsp;</strong></p>
<ul data-sourcepos="44:5-57:0">
<li style="text-align: justify;" data-sourcepos="44:5-57:0">Iterate through each line defined in the data input.
<ul data-sourcepos="45:9-57:0">
<li style="text-align: justify;" data-sourcepos="45:9-45:94">Clear the <em>\coords</em> token for storing data point coordinates for the current line.</li>
<li style="text-align: justify;" data-sourcepos="46:9-48:97">Loop through each data point for the current line.
<ul data-sourcepos="47:13-48:97">
<li data-sourcepos="47:13-47:113">Calculate the data point value based on the line number and data point index within the data array.</li>
<li data-sourcepos="48:13-48:97">Add the calculated X (data point number) and Y (data value) to the <em>\coords</em>&nbsp;token.</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="49:9-53:86">Define a plotting command with the following properties:
<ul data-sourcepos="50:13-53:86">
<li data-sourcepos="50:13-50:126">Set line color based on a loop counter (e.g., rgbColor1 for the first line, rgbColor2&nbsp;for the second, etc.).</li>
<li data-sourcepos="51:13-51:67">Set the marker style to an asterisk (*) for each data point.</li>
<li data-sourcepos="52:13-52:36">Set the line width to 2 pt.</li>
<li data-sourcepos="53:13-53:86">Specify the coordinates for the line using the expanded <em>\coords</em>&nbsp;token.</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="54:9-54:69">Execute the plotting command to draw the line on the graph.</li>
<li style="text-align: justify;" data-sourcepos="55:9-55:84">Add a legend label based on the corresponding legend entry from the input.</li>
<li style="text-align: justify;" data-sourcepos="56:9-57:0">Clear the <em>\coords</em> token to prepare for storing the coordinates of the next line.</li>
</ul>
</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="58:1-60:0">
<p data-sourcepos="58:4-58:18"><strong>Add Legend:</strong></p>
<ul data-sourcepos="59:5-60:0">
<li data-sourcepos="59:5-60:0">Add a legend box with its position and style options at a specified location (e.g., left side center).</li>
</ul>
</li>
<li data-sourcepos="61:1-63:0">
<p style="text-align: justify;" data-sourcepos="61:4-61:28"><strong>End TikZ Environment:</strong></p>
<ul data-sourcepos="62:5-63:0">
<li style="text-align: justify;" data-sourcepos="62:5-63:0">Close the TikZ picture environment.</li>
</ul>
</li>
</ol>
<p id="bkmrk-%C2%A0-6"></p>
<h2 id="bkmrk-work-flow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="1241" contenteditable="false" id="bkmrk--1"><img id="bkmrk--2" src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/BDNnD12rxu6Kp9Q6-drawing-36-1713271225.png"></div>
<p id="bkmrk-%C2%A0-7"></p>

<p id="bkmrk--3"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<ul id="bkmrk-%231----height-and-wid">
<li class="null"><strong>#1 -- Height and Width of the graph in (cm)</strong></li>
<li class="null"><strong>#2 -- Y axis minimum and maximum values </strong>- To adjust the maximum value of the y axis, range from 0 to 100.</li>
<li class="null"><strong>#3 -- X axis tick labels with separations</strong> - Labels for the x-axis plots [For example, months like Jan, Feb etc..,].</li>
<li class="null"><strong>#4 -- Y axis tick labels with separations </strong>- Labels for the y-axis plots based on the percentage to reduce the space.</li>
<li class="null"><strong>#5 -- X-axis Label</strong> - Label for the x axis [Months]</li>
<li class="null"><strong>#6 -- Y-axis Label</strong> - Label for the y axis [Test Consumption in %]</li>
<li class="null"><strong>#7 -- Graph legends </strong>- Representation of the bars [Math and Science]</li>
<li class="null"><strong>#8 -- No. of Graph lines, No. of plots and Coordinates of the graph<br>Array 0 - No. of Graph lines </strong>- Number of subjects.<strong><br>Array 1 - No. of plots </strong>- Number of months<strong><br>Array 2 - Coordinates of the graph up to </strong>- Consumption percent belonging to the particular month<strong><br>Array n - Coordinates of the graph</strong></li>
<li class="null"><strong>#9 -- Title of the graph</strong></li>
</ul>
<p id="bkmrk-%C2%A0-8"></p>
<h2 id="bkmrk-output-of-the-latex-"><span style="text-decoration: underline;"><strong>Output of the LaTeX Code</strong></span></h2>
<p id="bkmrk--4"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/4YyxsvKbtNoyp56Q-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/4YyxsvKbtNoyp56Q-image.png" alt="image.png" width="483" height="294"></a></p>
<p id="bkmrk-%C2%A0-9"></p>
<p id="bkmrk--5"><br></p>


## LaTex Overleaf Project Link:

Only view the project **[PROJECT LINK](https://www.overleaf.com/read/dvqvjbtrqrqp#32b240)**




## NOTICE:
 
- If you don't provide the line colors, it does take the default value; all lines appear in the same color.
- If you have multiple lines, don't forget to include the legend names of the individual lines.
- Whenever you want, you can uncommand the 'every node near coord' line (that is, line no. 92), which changes the position of the node value near the coordinates.

## Short Note for Tokens:

**Token Registers:**

- A token register is a special type of variable in TeX and LaTeX that can hold a sequence of tokens.
- Tokens can be characters, control sequences, or other special symbols.
Unlike macros, token registers do not expand when used.

**Syntax:**

- To create a new token register, you use the \newtoks command followed by the name of the register.

    For example: \newtoks\mytokens

Assigning Values:
- After declaring a token register, you can assign values to it using the syntax: \mytokens={...}.
- The tokens inside the braces {...} are stored in the token register.
- For example: \mytokens={123}

**Appending Tokens:**

- There is no direct provision for appending tokens to an existing token register.
- To append tokens, you can exploit the way assignments work in TeX.
For example, to append “abc” to an existing token register \mytokens, you can do:

      \mytokens=\expandafter{\the\mytokens abc}


## References:

- [Plotting the Coordinates](https://tex.stackexchange.com/questions/393934/how-to-use-a-command-inside-addplot-options)

- [Constructing coordinates using foreach loop](https://tex.stackexchange.com/questions/684978/defining-coordinates-in-foreach)

- [Tex Tokens](https://www.overleaf.com/learn/latex/Articles/What_is_a_TeX_token_list)

- [\newtoks and \the commands](https://tex.stackexchange.com/questions/639301/using-foreach-loop-for-generating-sets-of-coordinates-for-const-plot-mark-mid)