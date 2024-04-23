<h1 id="bkmrk-contribution-chart"><strong><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);">Contribution Chart</span></strong></h1>
<p id="bkmrk-%C2%A0"></p>

<p id="bkmrk-%C2%A0-1"></p>
<ul id="bkmrk-a-contribution-chart">
<li class="null" style="text-align: justify;">A <strong>Contribution Chart</strong>, also known as a contribution graph, visually represents a user&rsquo;s contributions over time to showcasing the user&rsquo;s work and activity levels.</li>
<li class="null" style="text-align: justify;">The chart uses a grid format, often resembling a calendar, where each day is represented by a square.</li>
<li class="null" style="text-align: justify;">The squares are shaded or colored differently to reflect the user's contribution level on that day. More frequent contributions might be shown as darker shades or brighter colors.</li>
</ul>
<p id="bkmrk--1"></p>
<h2 id="bkmrk-purpose"><span style="text-decoration: underline;"><strong>Purpose</strong></span></h2>
<ul id="bkmrk-for-activity-trackin">
<li style="text-align: justify;" data-sourcepos="13:1-13:132">For activity tracking, it provides a quick overview of a user's contribution history, highlighting periods of high or low engagement.</li>
<li class="null" style="text-align: justify;">For example, the contribution chart gives the teachers a better visual experience of their DCP update status over time.</li>
</ul>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-requirements"><span style="text-decoration: underline;"><strong>Requirements</strong></span></h2>
<ul id="bkmrk-height-and-width---t">
<li class="null" style="text-align: justify;"><strong>Height and Width</strong> - The heights and widths are used to adjust the size of the graph layout. You can specify the height and width in centimeters (cm), millimeters (mm), or points (pt).</li>
<li class="null" style="text-align: justify;"><strong>Width of the box - </strong>To adjust the width of all boxes and reduce the whitespace to fill the overall layout.</li>
<li class="null" style="text-align: justify;"><strong>Labels -</strong> To individually identify the groups of boxes that represent the month with a day.<br></li>
<li class="null" style="text-align: justify;"><strong>Color intensity - </strong>For visually separate the day with more activity and a day with less activity.</li>
<li class="null" style="text-align: justify;"><strong>Start and End points - </strong>The starting month or a week in a specific month and the ending month or a week in a specific month.</li>
<li class="null" style="text-align: justify;"><strong>Details of the chart - </strong>The user's details of the data in a chart, like the teacher's details.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-resizing-the-chart-l">
<li class="null" style="text-align: justify;">Resizing the chart layout may cause it to overlap with other nodes.</li>
</ul>
<p id="bkmrk--2"></p>
<h2 id="bkmrk-latex-link"><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h2>
<h5 id="bkmrk-lapis-report---%3E-con" style="padding-left: 40px;">Intern Works --&gt; Charts --&gt; Contribution Chart --&gt; Contribution Chart.tex</h5>
<p id="bkmrk-%C2%A0-4"></p>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-defining-the-variabl" data-sourcepos="23:1-73:0">
<li data-sourcepos="31:1-33:0">
<p data-sourcepos="31:4-31:45"><strong>Defining the variables:</strong></p>
<ul data-sourcepos="32:5-33:0">
<li data-sourcepos="32:5-33:0">Extract box width, height, corner rounding, number of months, month names, fitting information, and data matrix from the input arguments.</li>
</ul>
</li>
<li data-sourcepos="34:1-37:0">
<p data-sourcepos="34:4-34:28"><strong>Define Custom Colors:</strong></p>
<ul data-sourcepos="35:5-37:0">
<li data-sourcepos="35:5-35:100">Define three colors (<code>color1</code>,&nbsp;<code>color2</code>,&nbsp;<code>color3</code>) to represent different update count ranges.</li>
<li data-sourcepos="36:5-37:0">Define a color (<code>noUpdateColor</code>) for weekdays with no updates.</li>
</ul>
</li>
<li data-sourcepos="38:1-42:0">
<p data-sourcepos="38:4-38:30"><strong>Begin TikZ Environment:</strong></p>
<ul data-sourcepos="39:5-42:0">
<li data-sourcepos="39:5-39:60">Start a&nbsp;<code>tikzpicture</code>&nbsp;environment to define the chart.</li>
<li data-sourcepos="40:5-40:77">Define box styles, label styles, and a style for boxes with no updates.</li>
<li data-sourcepos="41:5-42:0">Set the overall chart scale using the&nbsp;<code>scale</code>&nbsp;factor.</li>
</ul>
</li>
<li data-sourcepos="43:1-45:0">
<p data-sourcepos="43:4-43:30"><strong>Display Weekday Labels:</strong></p>
<ul data-sourcepos="44:5-45:0">
<li data-sourcepos="44:5-45:0">Use a loop to display weekday names (Sun, Mon, Tue, etc.) on the x-axis.</li>
</ul>
</li>
<li data-sourcepos="46:1-48:0">
<p data-sourcepos="46:4-46:36"><strong>Loop Through Months and Data:</strong></p>
<ul data-sourcepos="47:5-48:0">
<li data-sourcepos="47:5-48:0">Use a nested loop to iterate through each month and its corresponding data (update counts for weekdays).</li>
</ul>
</li>
<li data-sourcepos="49:1-54:0">
<p data-sourcepos="49:4-49:28"><strong>Calculate Fill Color:</strong></p>
<ul data-sourcepos="50:5-54:0">
<li data-sourcepos="50:5-54:0">Inside the loop, calculate a fill color for the current box based on the update count:
<ul data-sourcepos="51:9-54:0">
<li data-sourcepos="51:9-51:53">High update count (above 85) gets&nbsp;<code>color3</code>.</li>
<li data-sourcepos="52:9-52:64">Medium update count (between 45 and 85) gets&nbsp;<code>color2</code>.</li>
<li data-sourcepos="53:9-54:0">Low update count (below 45) gets&nbsp;<code>color1</code>.</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="55:1-63:0">
<p data-sourcepos="55:4-55:18"><strong>Draw Boxes:</strong></p>
<ul data-sourcepos="56:5-63:0">
<li data-sourcepos="56:5-63:0">Create a colored box for each update count value using the calculated fill color.
<ul data-sourcepos="57:9-63:0">
<li data-sourcepos="57:9-59:108">For the first row and column (month labels and weekday labels):
<ul data-sourcepos="58:13-59:108">
<li data-sourcepos="58:13-58:71">If it's Sunday (update count 0), fill the box with white.</li>
<li data-sourcepos="59:13-59:108">Otherwise, fill the box with the calculated color and display the update count within the box.</li>
</ul>
</li>
<li data-sourcepos="60:9-63:0">For other weekdays:
<ul data-sourcepos="61:13-63:0">
<li data-sourcepos="61:13-61:111">If it's a weekday with no updates (update count 0), use the&nbsp;<code>noupdate</code>&nbsp;style with a grid pattern.</li>
<li data-sourcepos="62:13-63:0">Otherwise, fill the box with the calculated color and display the update count within the box.</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="64:1-70:0">
<p data-sourcepos="64:5-64:39"><strong>Group and Display Month Labels:</strong></p>
<ul data-sourcepos="65:5-70:0">
<li data-sourcepos="65:5-70:0">Use another loop to iterate through each month.
<ul data-sourcepos="66:9-70:0">
<li data-sourcepos="66:9-66:70">Get the corresponding month name from the&nbsp;<code>monthnames</code>&nbsp;list.</li>
<li data-sourcepos="67:9-67:84">Get the fitting information (grouping row number) from the&nbsp;<code>fitting</code>&nbsp;list.</li>
<li data-sourcepos="68:9-68:89">Create a dummy element (<code>\node</code>) to determine the position for the month label.</li>
<li data-sourcepos="69:9-70:0">Place the month label to the left of the dummy element based on its position.</li>
</ul>
</li>
</ul>
</li>
</ol>
<p id="bkmrk-%C2%A0-5"></p>
<h2 id="bkmrk-workflow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="1252" contenteditable="false" id="bkmrk--3"><img id="bkmrk--4" src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/XqOF4JEKCK3LGJLE-drawing-36-1713351877.png"></div>
<p id="bkmrk-%C2%A0-6"></p>
<p id="bkmrk--5"></p>
<p id="bkmrk-%C2%A0-8"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<p id="bkmrk-%C2%A0-9"><strong>#1 -- Width and Height of the boxes</strong><br><strong>#2 -- Corner radius of the boxes</strong><br><strong>#3 -- Scale value - </strong>Resizing the layout, value must be greater than 0.6&nbsp;<br><strong>#4 -- No of months</strong><br><strong>#5 -- Month names - </strong>In an individual array format like { {"Jan"}, {"Feb"} }<br><strong>#6 -- Group names like (1)(2) ... with at least four, represents the weeks in a month</strong><br><strong>#7 -- Week wise data array</strong><br><strong>#8 -- Color of the box</strong></p>
<p id="bkmrk--6"></p>
<h2 id="bkmrk-output-of-the-latex-"><span style="text-decoration: underline;"><strong>Output of the LaTeX Code</strong></span></h2>
<p id="bkmrk--7"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/Y16uIp3QRqWVYhlt-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/Y16uIp3QRqWVYhlt-image.png" alt="image.png" width="381" height="556"></a></p>
<p id="bkmrk-%C2%A0-13"></p>

### Note:
- Above 85 --> Green
- Below 85 and Above 45 --> Yellow
- Below 45 --> Red
- If incase zero updates --> grid pattern with blue color

