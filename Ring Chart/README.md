<h1 id="bkmrk-ring%C2%A0chart"><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>Ring&nbsp;</strong></span><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>Chart</strong></span></h1>
<p id="bkmrk-%C2%A0"></p>
<ul id="bkmrk-a-ring-chart%2C-also-k">
<li class="null" style="text-align: justify;">A <strong>Ring Chart</strong>, also known as a <strong>Donut Chart or Pie Chart</strong>, is a type of data visualization that displays information in a concentric circular format.</li>
<li style="text-align: justify;">A ring chart represents data using segments arranged in a circular manner.&nbsp;Each segment corresponds to a proportion of the whole, with the outer ring representing 100% of the data.</li>
<li style="text-align: justify;">The size of each segment is proportional to the data it represents.</li>
</ul>
<p id="bkmrk-%C2%A0-1"></p>
<h2 id="bkmrk-purpose"><span style="text-decoration: underline;"><strong>Purpose</strong></span></h2>
<ul id="bkmrk-ring-charts-are-usef">
<li class="null" style="text-align: justify;">Ring charts are useful for comparing the relative sizes of different categories within a whole. They allow you to visualize the distribution of data across segments.</li>
<li class="null" style="text-align: justify;">Ring charts often display percentages or proportions for each segment.</li>
<li class="null" style="text-align: justify;">For example, the distribution of different types of responses or issues encountered by students in a class with various subjects is then classified into percentages of correct answers, concept issues, careless mistakes, critical thinking issues, and learn later categories.</li>
</ul>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-requirements"><strong><span style="text-decoration: underline;">Requirements</span></strong></h2>
<ul id="bkmrk-">
<li class="null"><strong>Radius of the circles -&nbsp;</strong>To adjust the overall height and width of the chart parallelly by resizing the inner and outer radius of the circle.<br></li>
<li class="null"><strong>Bar Labels -&nbsp;</strong>To provide the descriptive names for the individual sections.<br></li>
<li class="null"><strong>Title -&nbsp;</strong>To provide the name for the chart.<br></li>
<li class="null"><strong>Colors -&nbsp;</strong>The<strong>&nbsp;</strong>colors are used to differentiate the individual sections, like the correct answer, the concept issue, etc.,.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-in-the-ring-chart%2C-t">
<li class="null" style="text-align: justify;">In the ring chart, the upper portion of the ring has section labels that overlap with each other.</li>
<li class="null" style="text-align: justify;">Overflow happens when we feed too many concept names belonging to each section of items.</li>
<li class="null" style="text-align: justify;">If you use the scale property to size the layout, then the ring chart and the concept names overlap with each other.</li>
</ul>
<p id="bkmrk--1"></p>
<h2 id="bkmrk-latex-link"><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h2>
<h5 id="bkmrk-lapis-report---%3E-mis" style="padding-left: 40px; text-align: justify;">Intern Works --&gt; Charts --&gt; Pie Chart --&gt; Pie Chart - Mistake Analysis.tex</h5>
<p id="bkmrk-%C2%A0-4"></p>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-define-the-variables" data-sourcepos="23:1-64:0">
<li data-sourcepos="34:1-36:0">
<p data-sourcepos="34:4-34:45"><strong>Define the variables:</strong></p>
<ul data-sourcepos="35:4-36:0">
<li data-sourcepos="35:4-36:0">Extract the label, percentages (as a list), item counts (as a list), and item groups (as a list of lists) from the input arguments.</li>
</ul>
</li>
<li data-sourcepos="37:1-39:0">
<p data-sourcepos="37:4-37:21"><strong>Define Colors:</strong></p>
<ul data-sourcepos="38:4-39:0">
<li data-sourcepos="38:4-39:0">Define colors for chart elements: cell green, cell red, heading color, and white.</li>
</ul>
</li>
<li data-sourcepos="40:1-42:0">
<p data-sourcepos="40:4-40:43"><strong>Loop Through Percentages and Counts:</strong></p>
<ul data-sourcepos="41:4-42:0">
<li data-sourcepos="41:4-42:0">Loop through the provided percentages and item counts, storing the values for each category (careless mistakes, concepts issue, etc.) in separate variables.</li>
</ul>
</li>
<li data-sourcepos="43:1-50:0">
<p data-sourcepos="43:4-43:24"><strong>Draw Wheel Chart:</strong></p>
<ul data-sourcepos="44:4-50:0">
<li data-sourcepos="44:4-50:0">Create a wheel chart using the&nbsp;<code>wheelchart</code>&nbsp;package.
<ul data-sourcepos="45:7-50:0">
<li data-sourcepos="45:7-45:101">Define the data source (<code>\WCvarC</code>) and percentages (<code>\WCperc</code>) based on the extracted values.</li>
<li data-sourcepos="46:7-46:84">Set options for line styles, radius, and precision of displayed percentages.</li>
<li data-sourcepos="47:7-48:103">Populate the chart with slices for each category and its corresponding percentage value:
<ul data-sourcepos="48:11-48:103">
<li data-sourcepos="48:11-48:103">Label format: "{percentage}%/{color}/{category name}" (e.g., "6.16%/red/Careless Mistake").</li>
</ul>
</li>
<li data-sourcepos="49:7-50:0">Add content in the center of the chart using a node positioned at (0,0).</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="66:1-71:0">
<p data-sourcepos="66:4-66:41"><strong>Left Minipage (Mistake Breakdown):</strong></p>
<ul data-sourcepos="67:5-71:0">
<li data-sourcepos="67:5-67:54">Create a minipage for the left half of the page.</li>
<li data-sourcepos="68:5-68:67">List mistake categories with their corresponding percentages.</li>
<li data-sourcepos="69:5-71:0">For each category, iterate through the corresponding mistake list using a&nbsp;<code>foreach</code>&nbsp;loop.
<ul data-sourcepos="70:9-71:0">
<li data-sourcepos="70:9-71:0">Extract each mistake description from the nested list and display it as an item.</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="72:1-75:0">
<p data-sourcepos="72:5-72:42"><strong>Right Minipages (Mistake Details):</strong></p>
<ul data-sourcepos="73:5-75:0">
<li data-sourcepos="73:5-73:98">Create three minipages for the right half of the page, each representing a mistake category.</li>
<li data-sourcepos="74:5-75:0">Within each minipage, list the detailed descriptions of the mistakes belonging to that category using the same&nbsp;<code>foreach</code> loop approach.</li>
</ul>
</li>
</ol>
<p id="bkmrk--2"></p>
<h2 id="bkmrk-workflow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="1250" contenteditable="false" id="bkmrk--3"><img id="bkmrk--4" src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/zMA4HsQO3u6xlZlQ-drawing-36-1713343722.png"></div>
<p id="bkmrk-%C2%A0-5"></p>
<p id="bkmrk-%C2%A0-6"></p>
<p id="bkmrk--5"></p>
<p id="bkmrk--6"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<ul id="bkmrk-%231----chart-title---">
<li class="null" style="text-align: justify;"><strong>#1 -- Chart Title - Descriptive name of the chart </strong>[6, Math]<br></li>
<li class="null" style="text-align: justify;"><strong>#2 -- Percentage value of each category</strong><br></li>
<li class="null" style="text-align: justify;"><strong>#3 -- Count of the concepts belonging to each category</strong></li>
<li class="null" style="text-align: justify;"><strong>#4 -- Array of concept names belonging to each category - </strong>{ {&lt;concept names&gt;}, {&lt;concept names&gt;}, {&lt;concept names&gt;}, {&lt;concept names&gt;} }</li>
</ul>
<p id="bkmrk--7"></p>
<h2 id="bkmrk-output-of-the-latex-"><span style="text-decoration: underline;"><strong>Output of the LaTeX Code</strong></span></h2>
<p id="bkmrk--8"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/vAEhvLsmkfkHbeHm-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/scaled-1680-/vAEhvLsmkfkHbeHm-image.png" alt="image.png" width="569" height="288"></a></p>
<p id="bkmrk-%C2%A0-7"></p>