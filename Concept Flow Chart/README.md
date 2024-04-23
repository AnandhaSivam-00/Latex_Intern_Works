<h1 id="bkmrk-concept-flow-chart"><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>Concept Flow Chart</strong></span></h1>
<p id="bkmrk-%C2%A0"></p>
<h2 id="bkmrk-purpose"><span style="text-decoration: underline;"><strong>Purpose</strong></span></h2>
<ul id="bkmrk-the-purpose-of-this-">
<li class="null" style="text-align: justify;">The purpose of this chart is to visualize the performance of students in various mathematical topics.</li>
<li class="null" style="text-align: justify;">Each node represents a different math topic, and the colors indicate the performance levels of students: green for above 80%, yellow for between 60% and 80%, and purple for below 60%.</li>
<li class="null" style="text-align: justify;">The numbers in each node show the total number of students who scored in those respective ranges.</li>
</ul>
<p id="bkmrk-%C2%A0-1"></p>
<h2 id="bkmrk-requirements"><span style="text-decoration: underline;"><strong>Requirements</strong></span></h2>
<ul id="bkmrk-height-and-width---t">
<li class="null"><strong>Height and Width</strong> - The heights and widths are used to adjust the size of the node layout. You can specify the height and width in centimeters (cm), millimeters (mm), or points (pt).</li>
<li class="null"><strong>Width of the box -&nbsp;</strong>To adjust the width of all boxes and reduce the whitespace to fill the overall layout.</li>
<li class="null"><strong>Labels -</strong> To individually identify the boxes that represent the concept names.<br></li>
<li class="null"><strong>Legends - </strong>It describes what is the purpose of the node and the two circles.</li>
<li class="null"><strong>Color fill - </strong>Based on the conditions, the color circles are filled with colors.</li>
</ul>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-the-nodes-overflow-i">
<li class="null" style="text-align: justify;">The nodes overflow in the page layout when we feed too much data.</li>
<li class="null" style="text-align: justify;">The node containing the label has more than 3 lines, and then the label name overflows out of the node.</li>
<li class="null" style="text-align: justify;">Cannot able to resize the individual node.</li>
<li class="null" style="text-align: justify;">Manually directing each node to efficiently fill the page.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-latex-link"><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h2>
<h5 id="bkmrk-lapis-report---%3E%C2%A0" style="padding-left: 40px; text-align: justify;">Intern Works --&gt; Charts --&gt; Concept Flow Chart --&gt; Concept Flow Chart.tex</h5>
<p id="bkmrk-%C2%A0-4"></p>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-legend-definitions%3A-" data-sourcepos="7:1-52:24">
<li data-sourcepos="12:1-14:0">
<p data-sourcepos="12:4-12:26"><strong>Legend Definitions:</strong></p>
<ul data-sourcepos="13:4-14:0">
<li data-sourcepos="13:4-14:0"><code>\drawLegends</code>: Creates colored circles with labels representing performance categories (Above 80%, Between 60% and 80%, Below 60%).</li>
</ul>
</li>
<li data-sourcepos="15:1-17:0">
<p data-sourcepos="15:4-15:33"><strong>Flowchart Description Box:</strong></p>
<ul data-sourcepos="16:4-17:0">
<li data-sourcepos="16:4-17:0"><code>\flowchartDescription</code>: Creates a box displaying legends, total student count, and details for highlighted topics (circles).</li>
</ul>
</li>
<li data-sourcepos="21:1-27:0">
<p data-sourcepos="21:4-21:28"><strong>Node and Line Styles:</strong></p>
<ul data-sourcepos="22:4-27:0">
<li data-sourcepos="22:4-22:74"><code>block</code>: Defines the style for rectangular boxes representing topics.</li>
<li data-sourcepos="23:4-23:49"><code>node distance</code>: Sets spacing between nodes.</li>
<li data-sourcepos="24:4-24:58"><code>line</code>: Defines the style for lines connecting nodes.</li>
<li data-sourcepos="25:4-25:79"><code>ring</code>: Defines the style for circles representing performance in a topic.</li>
<li data-sourcepos="26:4-27:0"><code>ringhighlight*</code>: Styles for highlighted rings with different fill colors (yellow, blue, green) based on performance.</li>
</ul>
</li>
<li data-sourcepos="28:1-30:0">
<p data-sourcepos="28:4-28:20"><strong>Node Counter:</strong></p>
<ul data-sourcepos="29:4-30:0">
<li data-sourcepos="29:4-30:0">Tracks the number of nodes created in the flowchart.</li>
</ul>
</li>
<li data-sourcepos="31:1-41:0">
<p data-sourcepos="31:4-31:31"><strong><code>\connectnodes</code> Command:</strong></p>
<ul data-sourcepos="32:4-41:0">
<li data-sourcepos="32:4-32:54">Creates a new node connected to the previous one.</li>
<li data-sourcepos="33:4-37:44">Takes four arguments:
<ul data-sourcepos="34:7-37:44">
<li data-sourcepos="34:7-34:56">Ring count (e.g., 17) displayed within the ring.</li>
<li data-sourcepos="35:7-35:64">Percentage (e.g., 75) displayed to the left of the ring.</li>
<li data-sourcepos="36:7-36:49">Connection direction (<code>right</code>&nbsp;or&nbsp;<code>left</code>).</li>
<li data-sourcepos="37:7-37:44">Topic name displayed inside the box.</li>
</ul>
</li>
<li data-sourcepos="38:4-38:65">Positions the node based on the previous node and direction.</li>
<li data-sourcepos="39:4-39:104">Assigns a ring style (yellow, blue, or green) based on the percentage using conditional statements.</li>
<li data-sourcepos="40:4-41:0">Draws rings with percentage and topic name.</li>
</ul>
</li>
<li data-sourcepos="42:1-46:0">
<p data-sourcepos="42:4-42:26"><strong>Flowchart Creation:</strong></p>
<ul data-sourcepos="43:4-46:0">
<li data-sourcepos="43:4-43:116">Uses the&nbsp;<code>\connectnodes</code>&nbsp;command repeatedly to create nodes and connect them, building the flowchart structure.</li>
<li data-sourcepos="44:4-44:80">The second argument (percentage) is now explicitly provided for each topic.</li>
<li data-sourcepos="45:4-46:0">Some topics connect to nodes below them, demonstrating sub-topics.</li>
</ul>
</li>
<li data-sourcepos="47:1-51:0">
<p data-sourcepos="47:4-47:33"><strong>Flowchart Description Box:</strong></p>
<ul data-sourcepos="48:4-51:0">
<li data-sourcepos="48:4-48:56">Inserts the legend box with performance categories.</li>
<li data-sourcepos="49:4-49:34">Displays total student count.</li>
<li data-sourcepos="50:4-51:0">Provides details for highlighted topics (circles).</li>
</ul>
</li>
</ol>
<p id="bkmrk-%C2%A0-6"></p>
<h2 id="bkmrk-workflow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="1263" contenteditable="false" id="bkmrk-"><img id="bkmrk--1" src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/DynBCJvNVKvOLrb4-drawing-36-1713434921.png"></div>
<p id="bkmrk-%C2%A0-7"></p>
<p id="bkmrk-%C2%A0-8"></p>

<p id="bkmrk-%C2%A0-9"></p>
<p id="bkmrk-%C2%A0-10"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<ul id="bkmrk-%C2%A0the-%5Cconnectnodes-c">
<li class="null" style="font-weight: bold;">
<p><strong>&nbsp;The <code>\connectnodes</code> Command</strong></p>
<ul>
<li class="null"><strong>#1 --&nbsp; No. of Students -&nbsp;Total students belonging to the concept based on the performance</strong></li>
<li class="null"><strong>#2 --&nbsp; Percentage score</strong></li>
<li class="null"><strong>#3 -- Position of the node respect to the previous node</strong></li>
<li class="null"><strong>#4 -- Concept name for label</strong></li>
</ul>
</li>
<li class="null"><strong>The <code>\flowchartDescription</code></strong>&nbsp;<strong>Command</strong>
<ul>
<li class="null"><strong>#1 -- Space between the chart and legend</strong></li>
<li class="null"><strong>#2 -- Space between the legends&nbsp;</strong></li>
<li class="null"><strong>#3 -- Student count</strong></li>
</ul>
</li>
</ul>
<p id="bkmrk-%C2%A0-11"></p>
<h2 id="bkmrk-output-of-the-latex-"><span style="text-decoration: underline;"><strong>Output of the LaTeX Code</strong></span></h2>
<p id="bkmrk--2"><span style="text-decoration: underline;"><strong><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/kQgZT7tGBu3gHlnF-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/scaled-1680-/kQgZT7tGBu3gHlnF-image.png" alt="image.png" width="403" height="468"></a></strong></span></p>