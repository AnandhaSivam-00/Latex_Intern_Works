<h1 id="bkmrk-grouped-bar-graph"><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>Grouped Bar Graph</strong></span></h1>
<p id="bkmrk-%C2%A0"></p>
<ul id="bkmrk-a-grouped-bar-graph-">
<li class="null" style="text-align: justify;">A<strong> Grouped Bar Graph </strong>also called<strong> Clustered Bar Graph</strong> is one kind of bar graph used to make comparisons across different categories of data from a single or multiple groups.</li>
<li class="null" style="text-align: justify;">Grouped bar charts make it clear how categories (addition, subtraction, etc.., or different subject concepts) differ in value (score or test percentage) across different groups (classes and their sections). This can be useful for identifying areas that require improvement for the students in a class.</li>
</ul>
<p id="bkmrk-%C2%A0-1"></p>
<h2 id="bkmrk-purpose"><span style="text-decoration: underline;"><strong>Purpose</strong></span><br></h2>
<p id="bkmrk-grouped-bar-graphs-a" style="padding-left: 40px; text-align: justify;">Grouped bar graphs are used when two or more data points, like overall student counts in addition, subtraction, etc., or subject concepts are displayed side-by-side and grouped together under categories like class sections in a school on the same axis.</p>
<p id="bkmrk-%C2%A0-2" style="padding-left: 40px; text-align: justify;"></p>
<h2 id="bkmrk-requirements" style="text-align: justify;"><span style="text-decoration: underline;"><strong>Requirements</strong></span></h2>
<ul id="bkmrk-height-and-width--%C2%A0t">
<li class="null"><strong>Height and Width -&nbsp;</strong>The heights and widths are used to adjust the size of the graph layout. You can specify the height and width in centimeters (cm), millimeters (mm), or points (pt).</li>
<li class="null"><strong>Width of the Bars -&nbsp;</strong>To control the width of bars and specify the width of individual bars in a bar graph.</li>
<li class="null"><strong>Y Axis max value -&nbsp;</strong>The y axis maximum value is used to control the overlapping of the bars with a graph layout upper edge.</li>
<li class="null"><strong>X Tick Labels -&nbsp;</strong>Controls the labels displayed on the x-axis ticks.</li>
<li class="null"><strong>X and Y axis Labels -&nbsp;</strong>Providing a description or naming the axes of a graph or plot.</li>
<li class="null"><strong>Legends -&nbsp;</strong>To provide the descriptive names for the plots or a group of plots.</li>
<li class="null"><strong>Title -&nbsp;</strong>To provide the name for the graph.</li>
<li class="null"><strong>Bar Count - </strong>Number of bars belonging to each category.</li>
<li class="null"><strong>Coordinate points -&nbsp;</strong>The values that are used to plot the group of bars on the graph.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-the-graph-layout-ove">
<li class="null">The graph layout overflows in the page layout when we feed too much data.</li>
<li class="null">When the group contains too many bars, then it overlaps with other groups.</li>
</ul>
<p id="bkmrk-"></p>
<h2 id="bkmrk-latex-link"><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h2>
<h5 id="bkmrk--1" style="text-align: justify;">Intern Works --&gt; Charts --&gt; Grouped Bar Graphs --&gt; Grouped Bar Graph - Mistake in Basic Arithmetic.tex</h5>
<p id="bkmrk-%C2%A0-4"></p>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-define-axis-properti" data-sourcepos="27:1-72:0">
<li data-sourcepos="40:1-46:0">
<p data-sourcepos="40:4-40:30"><strong>Define Axis Properties:</strong></p>
<ul data-sourcepos="41:4-46:0">
<li data-sourcepos="41:4-46:0">Create an axis environment with a title, height, width, bar width, and other visual elements like grid lines, tick positioning, and labels.
<ul data-sourcepos="42:9-46:0">
<li data-sourcepos="42:9-42:97">Set Y-axis as the primary axis (<code>ybar</code>) and position labels on the top (<code>axis on top</code>).</li>
<li data-sourcepos="43:9-43:82">Set bar width and other axis properties similar to the previous example.</li>
<li data-sourcepos="44:9-44:64">Adjust Y-axis limits to accommodate the provided data.</li>
<li data-sourcepos="45:9-46:0">Configure legend position, style, and image code for visual representation of bars in the legend.</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="47:1-49:0">
<p data-sourcepos="47:4-47:28"><strong>Define Custom Colors:</strong></p>
<ul data-sourcepos="48:5-49:0">
<li data-sourcepos="48:5-49:0">Define colors for each data series (bar) in the graph.</li>
</ul>
</li>
<li data-sourcepos="50:1-53:0">
<p data-sourcepos="50:4-50:39"><strong>Loop Through Data Series (Bars):</strong></p>
<ul data-sourcepos="51:5-53:0">
<li data-sourcepos="51:5-53:0">Iterate through each data series (bar) in the provided data.
<ul data-sourcepos="52:9-53:0">
<li data-sourcepos="52:9-53:0"><strong>Clear Coordinates Token:</strong>&nbsp;Clear the&nbsp;<code>\coords</code>&nbsp;token before processing data points for the current series.</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="54:1-58:0">
<p data-sourcepos="54:4-54:40"><strong>Loop Through Categories (X-axis):</strong></p>
<ul data-sourcepos="55:5-58:0">
<li data-sourcepos="55:5-58:0">Iterate through each category (X-axis label) within the data for the current series.
<ul data-sourcepos="56:9-58:0">
<li data-sourcepos="56:9-56:129"><strong>Extract Data Point Value:</strong>&nbsp;Get the Y-axis value for the current category from the data array for the current series.</li>
<li data-sourcepos="57:9-58:0"><strong>Store Coordinates:</strong>&nbsp;Add the category position (adjusted slightly) and the Y-axis value to the&nbsp;<code>\coords</code>&nbsp;token.</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="59:1-62:0">
<p data-sourcepos="59:4-59:31"><strong>Define Plotting Command:</strong></p>
<ul data-sourcepos="60:5-62:0">
<li data-sourcepos="60:5-62:0">Create a plotting command to add the current series' data points to the graph.
<ul data-sourcepos="61:9-62:0">
<li data-sourcepos="61:9-62:0">Set&nbsp;<code>draw=none</code>&nbsp;to hide bar outlines and&nbsp;<code>fill</code>&nbsp;with the color to create filled bars.</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="63:1-65:0">
<p data-sourcepos="63:5-63:20"><strong>Plot Series:</strong></p>
<ul data-sourcepos="64:5-65:0">
<li data-sourcepos="64:5-65:0">Execute the plotting command to add the bars for the current series to the graph.</li>
</ul>
</li>
<li data-sourcepos="66:1-68:0">
<p data-sourcepos="66:5-66:32"><strong>Reset Coordinates Token:</strong></p>
<ul data-sourcepos="67:5-68:0">
<li data-sourcepos="67:5-68:0">Clear the&nbsp;<code>\coords</code> token again to prepare for processing data points for the next series.</li>
</ul>
</li>
</ol>
<p id="bkmrk-%C2%A0-5"></p>
<h2 id="bkmrk-workflow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="1247" contenteditable="false" id="bkmrk--2"><img src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/rx53P0raoMkP6XDb-drawing-36-1713337268.png"></div>
<p id="bkmrk--3"></p>
<h2 id="bkmrk-latex-code-and-its-o"><span style="text-decoration: underline;"><strong>LaTeX Code and its Output</strong></span></h2>
<p>&nbsp;</p>
<h5><strong>1. Based On X - Axis</strong></h5>
<pre id="bkmrk-%5Cdocumentclass%5Bborde"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=1.8cm,bottom=1.5cm,left=0.5cm,right=0.5cm, a4paper}
\usepackage{pgfplots}
\pgfplotsset{width=7cm,compat=1.18} 
\usepackage{sfmath}
\renewcommand*{\familydefault}{\sfdefault}

\newtoks \coords  % this command is must for tokenizing the inputs

\newcommand{\mistakeinbasicairthmatic}[8]{
    \def \barcoords{#7}    % No of bars, No of plots and Coordinates of the graph

    \pgfmathsetmacro{\numOfBars}{{\barcoords}[0]}     % No of bars
    \pgfmathsetmacro{\noOfCoords}{{\barcoords}[1]}     % No of plots
    
    \begin{tikzpicture}[scale = 0.8]
        \centering
        \begin{axis}[
            ybar, axis on top,
            ybar=0.3cm,  
            ymax=#8,
            height=#1 cm, 
            width=#2 cm,
            bar width=#3 cm,            
            tick align=outside,
            grid=both,
            grid style = dashed,
            major grid style={draw=none,opacity=1,dotted},
            minor x tick num = 1,
            yminorgrids=false,
            enlarge y limits={value=.1,upper},
            ymin=0, ymax=#8, % Adjusted to fit the new data
            axis x line*=bottom,
            axis y line*=right,
            y axis line style={opacity=0},
            tickwidth=0pt,
            enlarge x limits=0.3,  
            legend style={
                at={(0.5,-0.15)},
                anchor=north,
                legend columns=-1,
                /tikz/every even column/.append style={column sep=0.5cm},
                draw=none
            },
            legend image code/.code={
                \draw [] (0cm,-0.15cm) rectangle (0.15cm,0.15cm);
            },
            ylabel={#5},
            xticklabels={#4},
            xtick=data,
            nodes near coords={
                \pgfmathprintnumber[precision=0]{\pgfplotspointmeta}
            },
            % x tick label style={rotate=45, anchor=east},
        ]

        \colorlet{color1}{blue!30}
        \colorlet{color2}{green!50}
        \colorlet{color3}{gray!30}
        \colorlet{color4}{red!30}
        \colorlet{color5}{orange!30}

        \foreach \i in {1,...,\numOfBars}{     % Loop for Bars
            \coords{}
        
            \foreach \x in {0,...,\inteval{\noOfCoords-1}}{     % Loop for plots
                \pgfmathsetmacro{\eachpoint}{{\barcoords}[\i+1][\x]}
                \global\coords\expandafter{\expanded{\the\coords(\x+1,\eachpoint)}}
                % Declare the \coords as global and make it as tokens
            }
            \edef \plotting{ \noexpand
                \addplot[ 
                    draw=none, 
                    fill=color\i
                ] coordinates {
                    \the\coords     % Expand the tokens as a coordinates
                }; \noexpand
            }
            
            \plotting

            \renewcommand{\coords}{{}}  % Clear the \coords data for storing the other bar coords
        }


    \legend{#6}
  \end{axis}
\end{tikzpicture}
}

\begin{document}

% #1 -- Height of the graph
% #2 -- Width of the graph
% #3 -- Bar width
% #4 -- x tick label separations
% #5 -- y axis label
% #6 -- Graph legends
% #7 -- No of Graph bars in a group, No of plots and Coordinates of the graph
% Array 0 - No of bars
% Array 1 - No of plots
% Array 2 - Coordinates of the graph upto
% Array n - Coordinates of the graph
% #8 -- ymax value

\mistakeinbasicairthmatic{8}
    {17.5}
    {0.5}
    {Class 6, Class 7, Class 8}
    {Number of Students}
    {Addition,Subtraction,Multiplication,Division,Place Value}
    {
        {5},
        {3},
        {14,24,26},
        {16,18,21},
        {23,33,31},
        {32,23,39},
        {18,40,30}
    }
    {40}


\end{document}</code></pre>
<p id="bkmrk--4"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<ul id="bkmrk-%231----height-of-the-">
<li class="null" style="text-align: justify;"><strong>#1 -- Height of the graph in (cm)</strong></li>
<li class="null" style="text-align: justify;"><strong>#2 -- Width of the graph in (cm)</strong></li>
<li class="null" style="text-align: justify;"><strong>&nbsp;#3 -- Bar width</strong></li>
<li class="null" style="text-align: justify;"><strong>#4 -- X axis tick labels with separations&nbsp;</strong>- Labels for the group of x-axis plots [Class 6, Class 7, Class 8]</li>
<li class="null" style="text-align: justify;"><strong>#5 -- Y-axis Label&nbsp;</strong>- Label for the y axis [Number of Students]</li>
<li class="null" style="text-align: justify;"><strong>#6 -- Graph legends&nbsp;</strong>- Representation of the Bars [Addition, Subtraction, Multiplication, Division and Place Values]</li>
<li class="null" style="text-align: justify;"><strong>#7 -- No. of Bars, No. of plots and Coordinates of the graph,&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Array 0 - No. of bars in a group</strong><br><strong>Array 1 - No.of group of bars</strong> - Count of parameters like Class 6, Class7 and Class 8 <strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</strong><br><strong>Array 2 to n -</strong><strong>&nbsp;Coordinates of the graph&nbsp;</strong>- No. of students belonging to the particular category.</li>
<li class="null" style="text-align: justify;"><strong>#8 -- ymax value - </strong>For adjusting the y axis maximum value.<br></li>
</ul>
<p id="bkmrk--5"></p>
<h2 id="bkmrk-output-of-the-latex-"><span style="text-decoration: underline;"><strong>Output of the LaTeX Code</strong></span><br></h2>
<p id="bkmrk--6"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/3vZBllp3ByL8aGKX-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-03/scaled-1680-/3vZBllp3ByL8aGKX-image.png" alt="image.png" width="534" height="250"></a></p>
<p>&nbsp;</p>
<h5><strong>2. Based On Y - Axis</strong></h5>
<pre><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=1.8cm,bottom=1.5cm,left=0.5cm,right=0.5cm, a4paper}
\usepackage{pgfplots}
\pgfplotsset{width=10cm,compat=1.18} 
\usepackage{pgfplotstable}
\renewcommand*{\familydefault}{\sfdefault}
\usepackage{sfmath}

\newtoks \coords 


\newcommand{\ybargraph}[9]{
    \def \barcoords{#8}    % No of bars, No of plots and Coordinates of the graph

    \pgfmathsetmacro{\numOfBars}{{\barcoords}[0]}     % No of bars
    \pgfmathsetmacro{\noOfCoords}{{\barcoords}[1]}     % No of plots
    \centering
    \begin{tikzpicture}[scale=0.4]
                \begin{axis}[
                    width=#1 cm,
                    height=#2 cm,
                    bar width=#3 pt,
                    tick style={draw=none},
                    axis x line*=bottom,
                    axis y line*=left,
                    yticklabels={#5},
                    yticklabel style ={text width=#4 cm,align=center},
                    ytick=data,
                    xtick={0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30},
                    xbar,
                    xmin=0,
                    area legend,
                    xlabel={#6},
                    ylabel={Percentage(\%)},
                    nodes near coords,
                    nodes near coords style={font=\large},
                    nodes near coords align={horizontal},
                    legend style={at={(0.5,-0.25)}, draw=none, anchor=north,legend columns=-1,column sep=0.2cm},
                    xmajorgrids=true,
                    title=\textbf{#9}
                ]

        \colorlet{Color1}{blue!30}
        \colorlet{Color2}{green!50}
        \colorlet{Color3}{yellow!50}
        \colorlet{Color4}{red!30}

        \foreach \i in {1,...,\numOfBars}{     % Loop for Bars
            \coords{}
        
            \foreach \x in {0,...,\inteval{\noOfCoords-1}}{     % Loop for plots
                \pgfmathsetmacro{\eachpoint}{{\barcoords}[\i+1][\x]}
                \global\coords\expandafter{\expanded{\the\coords(\eachpoint, \x+1)}}
                % Declare the \coords as global and make it as tokens
            }
            \edef \plotting{ \noexpand
                \addplot[ 
                    draw=none, 
                    fill=Color\i
                ] coordinates {
                    \the\coords     % Expand the tokens as a coordinates
                }; \noexpand
            }
            
            \plotting

            \renewcommand{\coords}{{}}  % Clear the \coords data for storing the other bar coords
        }
        \legend{#7}
                \end{axis}
            \end{tikzpicture}
}

\begin{document}

% 1 -- Width
% 2 -- Height
% 3 -- bar width
% 4 -- text width
% 5 -- xticklabel
% 6 -- ylabel
% 7 -- legend
% 8 --{no. of legend}{no. of labels}{plots}
% 9 -- title


\ybargraph
{17}
{12}
{17}
{2.2}
{0\% to 20\%,20\% to 40\%,40\% to 60\%,60\% to 80\%,80\% to 100\%}
{No. of Students}
{Class 6AS, Class 6AC}
{
    {2},
    {5},
    {0,4,10,7,0},
    {0,14,8,8,2}
}
{Class 6 - Math}

\end{document}</code></pre>
<p>&nbsp;</p>
<h5><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h5>
<h5 style="padding-left: 40px;">Intern Works --&gt; Charts --&gt; Grouped Bar Graphs --&gt; Y-Axis Grouped Bar Graph.tex</h5>
<p>&nbsp;</p>
<h5>&nbsp;</h5>
<h5 id="bkmrk-%C2%A0-6"><span style="text-decoration: underline;"><strong>Output of the LateX Code</strong></span></h5>
<p><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/wIgA9aOr52qDI3yd-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/wIgA9aOr52qDI3yd-image.png" alt="image.png" width="334" height="253"></a></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h2 id="bkmrk-grouped-bar-graph-in"><span style="text-decoration: underline;"><strong>Grouped Bar Graph into Simple Bar Graph</strong></span></h2>
<p id="bkmrk-we-can-change-the-gr" style="padding-left: 40px; text-align: justify;">We can change the grouped bar graph into a single simple bar graph by passing a single parameter as an array.</p>
<pre id="bkmrk-%5Cmistakeinbasicairth"><code class="language-latex">\mistakeinbasicairthmatic{8}
    {17.5}
    {0.5}
    {Class 6, Class 7, Class 8}
    {Number of Students}
    {Addition}
    {
        {1},
        {3},
        {14,24,26}
    }
    {40}</code></pre>
<p id="bkmrk-%C2%A0-7"></p>
<h5 id="bkmrk-changed-parameters" style="text-align: justify;"><span style="text-decoration: underline;"><strong>Changed Parameters</strong></span></h5>
<ul id="bkmrk-change-the-graph-leg">
<li class="null">Change the graph legend parameter based on the array parameter passed.</li>
<li class="null">Change the number of bars to 1.</li>
<li class="null">Change the graph coordinates passed.</li>
</ul>
<p id="bkmrk-%C2%A0-8"></p>
<h2 id="bkmrk-output"><span style="text-decoration: underline;"><strong>Output</strong></span></h2>
<p id="bkmrk--7"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/CGQPdvnomHIIY9Wl-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/CGQPdvnomHIIY9Wl-image.png" alt="image.png" width="435" height="204"></a></p>
<p id="bkmrk-%C2%A0-9"></p>