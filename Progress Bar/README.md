<h1 id="bkmrk-progress-bar"><strong><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);" data-darkreader-inline-color="" data-darkreader-inline-bgcolor="">Progress Bar</span></strong></h1>
<p id="bkmrk-%C2%A0"></p>
<ul id="bkmrk-a%C2%A0progress-bar-is-a-">
<li>A&nbsp;<strong>progress bar</strong> is a visual representation used to track the completion status of a score or a percentage progress on a task or test or activity.</li>
<li>It typically consists of a horizontal bar that fills up as progress is made.</li>
</ul>
<p id="bkmrk-%C2%A0-1"></p>
<h2 id="bkmrk-purpose"><span style="text-decoration: underline;"><strong>Purpose</strong></span></h2>
<ul id="bkmrk-the-purpose-of-the-p">
<li>The purpose of the progress bar is to provide a clear visual indication of how much of the student has gained a score (in percentage) for individual concepts in a subject.</li>
</ul>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-requirements"><span style="text-decoration: underline;"><strong>Requirements</strong></span></h2>
<ul id="bkmrk-height-and-width-of-">
<li class="null"><strong>Height and width of the chart</strong> - The layout of the bar should be adjusted by using the height and width.</li>
<li class="null"><strong>Color of the bar&nbsp;</strong>- The color should be customizable based on the subject concept or certain criteria, like whether the color of the bar will change when the student's percentage is above 70%.</li>
<li class="null"><strong>Labels -&nbsp;</strong>It shows the details about each individual bar.</li>
<li class="null"><strong>Text width -&nbsp;</strong>The text should be adjustable to prevent it from overlapping other elements.</li>
<li class="null"><strong>Bar width -&nbsp;</strong>It is possible to increase and decrease the size of the bar to make the chart clean.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-if-working-with-a-sc">
<li class="null">If working with a scale property, the goal lines and ticks need to be adjusted.</li>
</ul>
<p id="bkmrk-"></p>
<h2 id="bkmrk-lapis-link"><span style="text-decoration: underline;"><strong>LaPIS Links</strong></span></h2>
<h5 id="bkmrk-lapis-report---%3E-pro" style="padding-left: 40px;">Intern Works --&gt; Charts --&gt; Progress Bar --&gt; Progress Bar 1.tex</h5>
<h5 id="bkmrk-lapis-report---%3E-pro-1" style="padding-left: 40px;">Intern Works --&gt; Charts --&gt; Progress Bar --&gt; Progress Bar 2.tex</h5>
<p id="bkmrk-%C2%A0-4"></p>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-defining-variables%3A-" data-sourcepos="20:1-62:0">
<li data-sourcepos="27:1-29:0">
<p data-sourcepos="27:4-27:45"><strong>Defining Variables:</strong></p>
<ul data-sourcepos="28:5-29:0">
<li data-sourcepos="28:5-29:0">Extract scale value (optional, defaults to 1), corner radius, bar width, goal value, percentage score, and concept name from the input arguments.</li>
</ul>
</li>
<li data-sourcepos="30:1-32:0">
<p data-sourcepos="30:4-30:21"><strong>Define Colors:</strong></p>
<ul data-sourcepos="31:4-32:0">
<li data-sourcepos="31:4-32:0">Create colors for the background (backgroundColor), progress bar fill (color1, color2, color3), tick marks (blacktick), and goal line (red).</li>
</ul>
</li>
<li data-sourcepos="36:1-38:0">
<p data-sourcepos="36:4-36:25"><strong>Style Definitions:</strong></p>
<ul data-sourcepos="37:5-38:0">
<li data-sourcepos="37:5-38:0">Define styles for labels, bars, plotting area, titles, and ticks (including goal line ticks) using properties like font size, minimum size, rounding corners, bar width, fill colors, and line styles.</li>
</ul>
</li>
<li data-sourcepos="39:1-41:0">
<p data-sourcepos="39:4-39:28"><strong>Calculate Fill Color:</strong></p>
<ul data-sourcepos="40:5-41:0">
<li data-sourcepos="40:5-41:0">Based on the percentage score, determine the appropriate fill color (color1, color2, color3) using conditional statements.</li>
</ul>
</li>
<li data-sourcepos="42:1-44:0">
<p data-sourcepos="42:4-42:32"><strong>Display Percentage Label:</strong></p>
<ul data-sourcepos="43:5-44:0">
<li data-sourcepos="43:5-44:0">Place a node with the percentage score and a percent sign at a specific location.</li>
</ul>
</li>
<li data-sourcepos="45:1-49:0">
<p data-sourcepos="45:4-45:17"><strong>Draw Bars:</strong></p>
<ul data-sourcepos="46:5-49:0">
<li data-sourcepos="46:5-49:0">Draw two bars:
<ul data-sourcepos="47:9-49:0">
<li data-sourcepos="47:9-47:60">A background bar with the&nbsp;<code>backgroundColor</code>&nbsp;fill.</li>
<li data-sourcepos="48:9-49:0">A progress bar with the calculated&nbsp;<code>fillColor</code>. The width is determined by the&nbsp;<code>bar width</code>&nbsp;argument.</li>
</ul>
</li>
</ul>
</li>
<li data-sourcepos="50:1-53:0">
<p data-sourcepos="50:5-50:19"><strong>Draw Ticks:</strong></p>
<ul data-sourcepos="51:5-53:0">
<li data-sourcepos="51:5-51:87">Loop from 1 to 9 to create minor tick marks along the bar using a&nbsp;<code>foreach</code>&nbsp;loop.</li>
<li data-sourcepos="52:5-53:0">Create a major tick mark at the end of the progress bar using a separate node with the&nbsp;<code>tick</code>&nbsp;style.</li>
</ul>
</li>
<li data-sourcepos="54:1-56:0">
<p data-sourcepos="54:5-54:23"><strong>Draw Goal Line:</strong></p>
<ul data-sourcepos="55:5-56:0">
<li data-sourcepos="55:5-56:0">Draw a dashed red line representing the goal value. The line position is calculated based on the goal value and bar width.</li>
</ul>
</li>
<li data-sourcepos="57:1-59:0">
<p data-sourcepos="57:5-57:22"><strong>Display Title:</strong></p>
<ul data-sourcepos="58:5-59:0">
<li data-sourcepos="58:5-59:0">Place a node with the concept name below the bar as the title.</li>
</ul>
</li>
</ol>
<p id="bkmrk--1"></p>
<h2 id="bkmrk-workflow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="" contenteditable="false" id="bkmrk--2"><br></div>
<div drawio-diagram="1253" contenteditable="false" id="bkmrk--3"><img id="bkmrk--4" src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/hkcDt9QpvbNKzEGe-drawing-36-1713361951.png"></div>
<p id="bkmrk-%C2%A0-5"></p>
<h2 id="bkmrk-latex-code"><span style="text-decoration: underline;"><strong>LaTeX Code</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{tikz}
\usepackage{geometry}
\usepackage{xcolor}
\usetikzlibrary{positioning, fit, shadings}
\geometry{top=1.8cm,bottom=1.5cm,left=0.5cm,right=0.5cm, a4paper}
\usepackage{progressbar}
\usepackage{pgfplots}
\usepackage{colortbl}
\pgfplotsset{compat=1.18}


\newcommand{\progressbars}[6]{
    \def \percent{#5}
    \def \reducedvalue{\percent*0.1}
    \def \tickheight{#3 + 0.85}

    % Defining colors
    \definecolor{color1}{RGB}{248, 131, 121}
    \definecolor{color2}{RGB}{251, 236, 93}
    \definecolor{color3}{RGB}{152, 251, 152}
    \definecolor{blacktick}{RGB}{96, 96, 96}
    \colorlet{backgroundColor}{gray!20}

    
    \begin{tikzpicture}[
        label/.style={  % Defining label style
            font=\small, 
            minimum size=5mm
        },
        bar/.style={    % Defining bar style
            draw=black,
            rounded corners=#2 pt
        },
        plotting/.style={
            xbar,
            bar width=#3 cm
        },
        title/.style={  % Defining bar title
            font=\large, 
            minimum size=5mm
        },
        tick/.style={   % Defining tick style
            draw=none, 
            rectangle, 
            minimum height=\tickheight cm, 
            minimum width=0.5mm, % To adjust big tick width
            fill=blacktick,
            color=blacktick
        },
        goalLine/.style={   % Goal line tick style
            thick, 
            dash dot, 
            color=red, 
            line width=1pt  % To adjust the goal line width
        },
        scale=#1
    ]

        % Setting the color based on the percentage value
        \ifnum \percent &gt; 85
            \pgfmathtruncatemacro\fillcolor{3}
        \else 
            \ifnum \percent &gt; 45
                \pgfmathtruncatemacro\fillcolor{2}
            \else 
                \pgfmathtruncatemacro\fillcolor{1}
            \fi
        \fi

        % Display the label
       \node[label] at (\reducedvalue,0.8) {\percent\%};

       % Bar with fills
       \draw[fill=backgroundColor, bar] plot[plotting] coordinates {(10,0)};
       \draw[fill=color\fillcolor, bar] plot[plotting] coordinates {(\reducedvalue,0)};

        % Adding ticks to the bars
        \foreach \i in {1,...,9} {
            \node[color=blacktick] at (\i, 0) {\scriptsize{$|$}};
        }
        
        \node[tick, inner sep=1pt] at (\reducedvalue, 0) {\footnotesize{$|$}};

        % Setting the Goal
        \draw[goalLine] (#4*0.1, #3-0.2) -- (#4*0.1, -#3+0.2);
        
        % Adding title of the bar
        \node[title] at (5,-1) {#6};
    \end{tikzpicture} \\
}

\begin{document}

% #1 -- Scale value [default value is 1]
% #2 -- Corner Radius in pt
% #3 -- Bar Width in cm
% #4 -- Goal value
% #5 -- Percentage score
% #6 -- Concept name

\progressbars
    {1}
    {2}
    {0.8}
    {80}
    {30}
    {Basics of Algebra}

\progressbars
    {1}
    {2}
    {0.8}
    {77}
    {68}
    {Knowing on numbers}

\progressbars
    {1}
    {2}
    {0.8}
    {40}
    {92}
    {Algebric Expressions}
\end{document}</code></pre>
<p id="bkmrk-%C2%A0-6"></p>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C-1"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{tikz}
\usepackage{geometry}
\usepackage{xcolor}
\usetikzlibrary{positioning, fit, shadings}
\geometry{top=1.8cm,bottom=1.5cm,left=0.5cm,right=0.5cm, a4paper}
\usepackage{progressbar}
\usepackage{pgfplots}
\usepackage{colortbl}
\pgfplotsset{compat=1.18}


\newcommand{\progressbars}[6]{
    \def \percent{#5}
    \def \reducedvalue{\percent*0.1}
    \def \tickheight{#3 + 0.85}

    % Defining colors
    \definecolor{color1}{RGB}{248, 131, 121}
    \definecolor{color2}{RGB}{251, 236, 93}
    \definecolor{color3}{RGB}{152, 251, 152}
    \definecolor{blacktick}{RGB}{96, 96, 96}

    
    \begin{tikzpicture}[
        label/.style={  % Defining label style
            font=\small, 
            minimum size=5mm
        },
        bar/.style={    % Defining bar style
            draw=black,
            rounded corners=#2 pt
        },
        shade/.style={  % Defining the bar shading styles 
            left color=color\fillcolor, 
            right color=white, 
            shading angle=90
        },
        plotting/.style={
            xbar,
            bar width=#3 cm
        },
        title/.style={  % Defining bar title
            font=\large, 
            minimum size=5mm
        },
        tick/.style={   % Defining tick style
            draw=none, 
            rectangle, 
            minimum height=\tickheight cm, 
            minimum width=0.5mm, 
            fill=blacktick,
            color=blacktick
        },
        goalLine/.style={   % Goal line tick style
            thick, 
            dash dot, 
            color=red, 
            line width=1pt
        },
        scale=#1
    ]

        % Setting the color based on the percentage value
        \ifnum \percent &gt; 85
            \pgfmathtruncatemacro\fillcolor{3}
        \else 
            \ifnum \percent &gt; 45
                \pgfmathtruncatemacro\fillcolor{2}
            \else 
                \pgfmathtruncatemacro\fillcolor{1}
            \fi
        \fi

        % Display the label
       \node[label] at (\reducedvalue,0.8) {\percent\%};

       % Bar with fills
       \shadedraw[shade, bar] plot[plotting] coordinates {(10,0)};

        % Adding ticks to the bars
        \foreach \i in {1,...,9} {
            \node[color=blacktick] at (\i, 0) {\scriptsize{$|$}};
        }
        
        \node[tick, inner sep=1pt] at (\reducedvalue, 0) {\footnotesize{$|$}};

        % Setting the Goal
        \draw[goalLine] (#4*0.1, #3-0.2) -- (#4*0.1, -#3+0.2);
        
        % Adding title of the bar
        \node[title] at (5,-1) {#6};
    \end{tikzpicture} \\
}

\begin{document}

% #1 -- Scale value [default value is 1]
% #2 -- Corner Radius in pt
% #3 -- Bar Width in cm
% #4 -- Goal value
% #5 -- Percentage score
% #6 -- Concept name

\progressbars
    {1}
    {2}
    {0.8}
    {80}
    {30}
    {Basics of Algebra}

\progressbars
    {1}
    {2}
    {0.8}
    {77}
    {68}
    {Knowing on numbers}

\progressbars
    {1}
    {2}
    {0.8}
    {40}
    {92}
    {Algebric Expressions}
\end{document}</code></pre>
<p id="bkmrk-%C2%A0-7"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<ul id="bkmrk-%231----scale-value-%5Bd">
<li class="null" style="text-align: justify;"><strong>#1 -- Scale value [default value is 1] - </strong>Resize the layout based on the environment</li>
<li class="null" style="text-align: justify;"><strong>#2 -- Corner Radius in pt - </strong>The corner curve of the bar in all ends</li>
<li class="null" style="text-align: justify;"><strong>#3 -- Bar Width in cm</strong></li>
<li class="null" style="text-align: justify;"><strong>#4 -- Goal value - </strong>To set a goal in the bar</li>
<li class="null" style="text-align: justify;"><strong>#5 -- Percentage score - </strong>Student score on the subject concept</li>
<li class="null" style="text-align: justify;"><strong>#6 -- Concept name</strong></li>
</ul>
<p id="bkmrk-%C2%A0-8"></p>
<h2 id="bkmrk-output-of-the-latex-"><span style="text-decoration: underline;"><strong>Output of the LaTeX Code</strong></span></h2>
<p id="bkmrk--5"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/RVEDKcJFd9s5Shfg-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/RVEDKcJFd9s5Shfg-image.png" alt="image.png" width="348" height="259"></a></p>
<p id="bkmrk--6"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/KaY3QeakpFaMLbsK-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/KaY3QeakpFaMLbsK-image.png" alt="image.png" width="347" height="260"></a></p>

## Note
- Color of the progress bar is changed automatically based on the percentage value
- Possible to set the goal for the each concept
