<h1 id="bkmrk-double-sided-bar-cha"><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>Bidirectional Bar Chart</strong></span></h1>
<p id="bkmrk-%C2%A0"></p>
<ul id="bkmrk-the-double-sided-bar">
<li class="null" style="text-align: justify;">The <strong>double-sided bar chart</strong>, or <strong>bidirectional bar chart</strong>, contains one bar on the right-hand side and one bar on the left-hand side.&nbsp;</li>
<li class="null" style="text-align: justify;">This type of chart helps visualize and compare two sets of data side by side with a common axis.&nbsp;</li>
</ul>
<p id="bkmrk-%C2%A0-1"></p>
<h2 id="bkmrk-purpose" style="text-align: justify;"><span style="text-decoration: underline;"><strong>Purpose</strong></span></h2>
<ul id="bkmrk-to-compare-the-math-">
<li class="null" style="text-align: justify;">To compare the math and science test results of the students in a class or a section.&nbsp;</li>
</ul>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-requirements"><span style="text-decoration: underline;"><strong>Requirements</strong></span></h2>
<ul id="bkmrk-height-and-width-of-">
<li class="null" style="text-align: justify;"><strong>Height and width of the chart</strong> - The layout should be adjusted by using the scale and shrink properties.</li>
<li class="null" style="text-align: justify;"><strong>Color of the bar </strong>- The color should be customizable based on the subject. One side of the bar has one color, and the other side of the bar has another color.</li>
<li class="null" style="text-align: justify;"><strong>Legends - </strong>It describes the group of bars belonging to which category (i.e., math or science).<br></li>
<li class="null" style="text-align: justify;"><strong>Labels - </strong>It shows the details about each individual bar. The bar on the left side and the bar on the right side share the same label.</li>
<li class="null" style="text-align: justify;"><strong>Title</strong> - Makes the chart more meaningful and understandable.</li>
<li class="null" style="text-align: justify;"><strong>Text width - </strong>The text should be adjustable to prevent it from overlapping other elements.</li>
<li class="null" style="text-align: justify;"><strong>Bar width - </strong>It is possible to increase and decrease the size of the bar to make the chart clean.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-when-resizing-the-ch">
<li class="null" style="text-align: justify;">When resizing the chart layout, except text, remaining all should be resized, but text remains in the same state.</li>
<li class="null" style="text-align: justify;">If the data point has a value between 1 and 10, then the name text and the percentage value overlap with each other.</li>
</ul>
<p id="bkmrk-%C2%A0-4"></p>
<h2 id="bkmrk-latex-link%3A"><span style="text-decoration: underline;"><strong>Latex Link</strong></span></h2>
<h5 id="bkmrk-%C2%A0lapis-report---%3E-bi">Intern Works --&gt; Charts --&gt; Bidirectional Bar Chart --&gt; Bidirectional Bar Chart.tex</h5>
<p id="bkmrk-%C2%A0-5"></p>
<p id="bkmrk-%C2%A0-6"></p>
<h2 id="bkmrk--1"></h2>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-define-variables%3A-ex" data-sourcepos="26:1-73:129">
<li data-sourcepos="35:1-37:0"><strong>Define Variables:</strong>
<ul data-sourcepos="26:1-73:129">
<li>Extract left and right labels, bar width, scale value, node distance for coordinate values, bar labels, number of plots, and data coordinates from the input arguments.</li>
</ul>
</li>
<li data-sourcepos="35:1-37:0">
<p data-sourcepos="35:4-35:28"><strong>Define Custom Colors:</strong></p>
<ul data-sourcepos="36:5-37:0">
<li data-sourcepos="36:5-37:0">Define colors for various elements like arrows, coordinate text, bars (left and right), and trend lines.</li>
</ul>
</li>
<li data-sourcepos="38:1-40:0">
<p data-sourcepos="38:4-38:30"><strong>Begin TikZ Environment:</strong></p>
<ul data-sourcepos="39:5-40:0">
<li data-sourcepos="39:5-40:0">Start a&nbsp;<code>\begin{tikzpicture}</code>&nbsp;environment to define the graph area.</li>
</ul>
</li>
<li data-sourcepos="41:1-43:0">
<p data-sourcepos="41:4-41:27"><strong>Define Label Styles:</strong></p>
<ul data-sourcepos="42:5-43:0">
<li data-sourcepos="42:5-43:0">Define styles for labels (general), left and right base bars, left and right bars with fill colors, and bar labels (X-axis).</li>
</ul>
</li>
<li data-sourcepos="44:1-46:0">
<p data-sourcepos="44:4-44:36"><strong>Define Left and Right Labels:</strong></p>
<ul data-sourcepos="45:5-46:0">
<li data-sourcepos="45:5-46:0">Place the left and right labels at the specified positions.</li>
</ul>
</li>
<li data-sourcepos="47:1-54:0">
<p data-sourcepos="47:4-47:41"><strong>Loop Through Left and Right Sides:</strong></p>
<ul data-sourcepos="48:5-54:0">
<li data-sourcepos="48:5-54:0">Iterate through two loops, one for the left side (index 1) and another for the right side (index 2).
<ul data-sourcepos="49:9-54:0">
<li data-sourcepos="49:9-49:135"><strong>Clear Coordinate Tokens:</strong>&nbsp;Clear the&nbsp;<code>\coords</code>&nbsp;and&nbsp;<code>\basecoords</code>&nbsp;tokens before processing data points for the current side.</li>
<li data-sourcepos="50:9-54:0"><strong>Loop Through Data Points:</strong>&nbsp;Iterate through each data point (plot) for the current side.
<ul data-sourcepos="51:13-54:0">
<li data-sourcepos="51:13-51:113"><strong>Extract Data Point Values:</strong>&nbsp;Calculate the Y-axis value from the data array for the current side.</li>
<li data-sourcepos="52:13-52:115"><strong>Reduce Coordinate Value:</strong>&nbsp;Reduce the data point value (optional scaling for better visualization).</li>
<li data-sourcepos="53:13-54:0"><strong>Store Coordinates:</strong>&nbsp;Based on the side (left or right), add the calculated X (reduced data point value, adjusted for position) and Y (plot number) values to the corresponding token (<code>\coords</code>&nbsp;for bars and&nbsp;<code>\basecoords</code>&nbsp;for baselines).</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="55:1-58:0">
<p data-sourcepos="55:4-55:36"><strong>Define Bar Plotting Commands:</strong></p>
<ul data-sourcepos="56:5-58:0">
<li data-sourcepos="56:5-56:115">Define a command to plot the left and right bars using the&nbsp;<code>\coords</code>&nbsp;token, style definitions, and bar width.</li>
<li data-sourcepos="57:5-58:0">Combine this command with another, defining the base bars (left and right) using the <code>\basecoords</code>&nbsp;token and corresponding style definitions.</li>
</ul>
</li>
<li data-sourcepos="59:1-61:0">
<p data-sourcepos="59:4-59:31"><strong>Plot Bars and Baselines:</strong></p>
<ul data-sourcepos="60:5-61:0">
<li data-sourcepos="60:5-61:0">Execute the combined bar plotting command to display the bars and baselines for the current side.</li>
</ul>
</li>
<li data-sourcepos="62:1-64:0">
<p data-sourcepos="62:5-62:32"><strong>Reset Coordinate Tokens:</strong></p>
<ul data-sourcepos="63:5-64:0">
<li data-sourcepos="63:5-64:0">Clear the&nbsp;<code>\coords</code>&nbsp;and&nbsp;<code>\basecoords</code>&nbsp;tokens again to prepare for processing data points for the next side (if applicable).</li>
</ul>
</li>
<li data-sourcepos="65:1-68:0">
<p data-sourcepos="65:5-65:41"><strong>Draw Center Axis and Trend Lines:</strong></p>
<ul data-sourcepos="66:5-68:0">
<li data-sourcepos="66:5-66:42">Draw a central axis with arrowheads.</li>
<li data-sourcepos="67:5-68:0">Draw dashed trend lines on both the left and right sides.</li>
</ul>
</li>
<li data-sourcepos="69:1-73:129">
<p data-sourcepos="69:5-69:32"><strong>Coordinate Value Labels:</strong></p>
<ul data-sourcepos="70:5-73:129">
<li data-sourcepos="70:5-73:129">Loop through both sides (left and right) and all data points (plots).
<ul data-sourcepos="71:9-73:129">
<li data-sourcepos="71:9-71:111"><strong>Extract Data Point Value:</strong>&nbsp;Get the Y-axis value from the data array for the current side and plot.</li>
<li data-sourcepos="72:9-72:86"><strong>Reduce Coordinate Value:</strong>&nbsp;Reduce the data point value (optional scaling).</li>
<li data-sourcepos="73:9-73:129"><strong>Adjust Label Position:</strong> Based on the side, data point value, and position of the base bar, calculate the appropriate</li>
</ul>
</li>
</ul>
</li>
</ol>
<p id="bkmrk--2"></p>
<h2 id="bkmrk-workflow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="1245" contenteditable="false" id="bkmrk--3"><img id="bkmrk--4" src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/rbyl5ysNVUqbz0Th-drawing-36-1713334271.png"></div>
<p id="bkmrk--5"></p>
<p id="bkmrk--6"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<ul id="bkmrk-%231----labels---subje">
<li class="null"><strong>#1 -- Labels </strong>- Subject Name&nbsp;</li>
<li class="null" style="font-weight: bold;"><strong>#2 -- Bar Width in cm&nbsp;</strong></li>
<li class="null"><strong>#3 -- Scale value in cm -&nbsp;</strong>Scale value to fit to the page</li>
<li class="null"><strong>#4 -- Distance of the node value from the coordinates in cm -&nbsp;</strong>Distance between percentage and bar</li>
<li class="null"><strong>#5 -- Bar Labels -&nbsp;</strong>Student Name</li>
<li class="null"><strong>#6 -- No.of Plots</strong> - No. of Studnet in the class&nbsp;</li>
<li class="null"><strong>#7 -- Coordinate values </strong>- Student score in math and science in order label provided { { },{ } }.</li>
</ul>
<p id="bkmrk--7"></p>
<h2 id="bkmrk-output-of-the-code"><span style="text-decoration: underline;"><strong>Output of the Code</strong></span></h2>
<p id="bkmrk--8"></p>
<p id="bkmrk--9"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/6I7B6CboORsl0TaX-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/scaled-1680-/6I7B6CboORsl0TaX-image.png" alt="image.png"></a></p>
<p id="bkmrk--10"></p>
<p id="bkmrk--11"></p>
<p id="bkmrk--12"></p>