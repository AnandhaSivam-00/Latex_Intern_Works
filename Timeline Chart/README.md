<h1 id="bkmrk-timeline-chart"><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>Timeline Chart</strong></span></h1>
<p id="bkmrk-%C2%A0"></p>
<ul id="bkmrk-a-timeline-chart-is-">
<li class="null" style="text-align: justify;">A <strong>Timeline Chart</strong> is also known as<strong> Gantt chart,</strong>&nbsp;uses a horizontal bar chart to visualize a plan over time, showing the schedule of tasks, their duration, dependencies between tasks, and the overall progress of the task or plan.</li>
<li class="null" style="text-align: justify;">A timeline chart is used to monitor the progress of the activities throughout a specific period of time, adjusting the curriculum as needed.</li>
</ul>
<p id="bkmrk-%C2%A0-1"></p>
<h2 id="bkmrk-purpose"><span style="text-decoration: underline;"><strong>Purpose</strong></span></h2>
<ul id="bkmrk-it-helps-in-organizi">
<li class="null" style="text-align: justify;">It helps in organizing the curriculum content and ensures that all necessary concepts are covered within the academic year.</li>
<li class="null" style="text-align: justify;">The chart can be used to schedule when each concept will be taught, allowing for a structured approach to the syllabus.</li>
<li class="null" style="text-align: justify;">It is also used to show how much percentage of the topic will be completed during the entire duration.</li>
</ul>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-requirements"><span style="text-decoration: underline;"><strong>Requirements</strong></span></h2>
<ul id="bkmrk-height-and-width%3A-ad">
<li style="text-align: justify;"><strong>Height and Width</strong>: Adjust the size of the Gantt chart. Specify the height and width in centimeters (cm), millimeters (mm), or points (pt) to fit the content and layout of your document.</li>
<li style="text-align: justify;"><strong>Bar Labels - </strong>Used to provide the description of how much day the particular task is taken.</li>
<li style="text-align: justify;"><strong>Legends</strong>: Include legends to provide descriptive names for different tasks or milestones within the Gantt chart.</li>
<li style="text-align: justify;"><strong>Title</strong>: Add a title to the Gantt chart to indicate the purpose, such as &ldquo;Academic Schedule for Class 6A&rdquo;.</li>
<li style="text-align: justify;"><strong>Color of the bar</strong>: Customize the color of the lines or bars to differentiate between subjects or to represent different classes or teachers.</li>
</ul>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-latex-link"><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h2>
<h5 id="bkmrk-lapis-report---%3E-tim" style="padding-left: 40px;">Intern Works --&gt; Charts --&gt; Time Line Chart --&gt; Timeline Chart.tex</h5>
<p id="bkmrk-%C2%A0-5"></p>
<p id="bkmrk-%C2%A0-6"></p>
<h2 id="bkmrk-procedure-%2F-algorith"><span style="text-decoration: underline;"><strong>Procedure / Algorithm of working</strong></span></h2>
<ol id="bkmrk-defining-the-variabl" data-sourcepos="29:1-71:0">
<li data-sourcepos="36:1-38:0">
<p style="text-align: justify;" data-sourcepos="36:4-36:45"><strong>Defining the Variables:</strong></p>
<ul style="text-align: justify;" data-sourcepos="37:5-38:0">
<li data-sourcepos="37:5-38:0">Extract title height, cell size, bar height, bar color, plan start date, plan end date, and task data from the input arguments.</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="39:1-41:0">
<p data-sourcepos="39:4-39:34"><strong>Weekday Label Redefinition:</strong></p>
<ul data-sourcepos="40:4-41:0">
<li data-sourcepos="40:4-41:0">Redefine the&nbsp;<code>\pgfcalendarweekdayletter</code>&nbsp;macro to display weekdays with different colors (Sunday in red).</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="42:1-45:0">
<p data-sourcepos="42:4-42:42"><strong>Custom Macro Definition (Internal):</strong></p>
<ul data-sourcepos="43:5-45:0">
<li data-sourcepos="43:5-43:86">Use&nbsp;<code>\makeatletter</code>&nbsp;and&nbsp;<code>\makeatother</code>&nbsp;to define a custom macro within the code.</li>
<li data-sourcepos="44:5-45:0">This macro allows setting custom concept names for tasks while automatically setting their progress to 100% (completed).</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="49:1-52:0">
<p data-sourcepos="49:4-49:23"><strong>Styling Options:</strong></p>
<ul data-sourcepos="50:5-52:0">
<li data-sourcepos="50:5-50:244">Set styles for various elements like vertical grid lines, title height, bar height, bar color, cell size, time format, bar label node fonts, label placement (inline), inline label node font and color, and title label font (commented out).</li>
<li data-sourcepos="51:5-52:0">Adjust label positioning for the rightmost bars using&nbsp;<code>labelposLeft</code>&nbsp;style.</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="53:1-55:0">
<p data-sourcepos="53:4-53:34"><strong>Define Start and End Dates:</strong></p>
<ul data-sourcepos="54:4-55:0">
<li data-sourcepos="54:4-55:0">Specify the plan start and end dates for the Gantt chart.</li>
</ul>
</li>
<li style="text-align: justify;" data-sourcepos="56:1-58:0">
<p data-sourcepos="56:4-56:33"><strong>Title Calendar Definition:</strong></p>
<ul data-sourcepos="57:5-58:0">
<li data-sourcepos="57:5-58:0">Define the title section to display month names, days, and weekdays using&nbsp;<code>\gantttitlecalendar</code>.</li>
</ul>
</li>
<li data-sourcepos="59:1-65:0">
<p style="text-align: justify;" data-sourcepos="59:5-59:18"><strong>Task Bars:</strong></p>
<ul data-sourcepos="60:5-65:0">
<li style="text-align: justify;" data-sourcepos="60:5-65:0">Loop through the provided task data and create a Gantt bar for each task using&nbsp;<code>\ganttbar</code>.
<ul data-sourcepos="61:9-65:0">
<li style="text-align: justify;" data-sourcepos="61:9-61:75">Set the concept name for the task using the&nbsp;<code>conceptName</code>&nbsp;option.</li>
<li style="text-align: justify;" data-sourcepos="62:9-62:46">Set the number of days for the task.</li>
<li style="text-align: justify;" data-sourcepos="63:9-63:91">If a specific start date is provided, use it. Otherwise, use the plan start date.</li>
<li style="text-align: justify;" data-sourcepos="64:9-65:0">Calculate the end date based on the start date and the number of days.</li>
</ul>
</li>
</ul>
</li>
</ol>
<p id="bkmrk-%C2%A0-7"></p>
<h2 id="bkmrk-workflow"><span style="text-decoration: underline;"><strong>Workflow</strong></span></h2>
<div drawio-diagram="1261" contenteditable="false" id="bkmrk--1"><img id="bkmrk--2" src="https://docs.learnbasics.fun/uploads/images/drawio/2024-04/X7ixU3JDMbbahqYZ-drawing-36-1713417616.png"></div>
<p id="bkmrk-%C2%A0-8"></p>
<p id="bkmrk--3"></p>
<h2 id="bkmrk-latex-code"><span style="text-decoration: underline;"><strong>LaTeX Code</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C"><code class="language-latex">\documentclass[11pt,a4paper]{article}
\usepackage{geometry}
\usepackage{tikz}
\usetikzlibrary{calc, calendar}
\usepackage{pgfgantt}
\geometry{top=1.8cm,bottom=1.5cm,left=0.5cm,right=0.5cm, a4paper}
\usepackage{pgfcalendar}
\usepackage[utf8]{inputenc}


\newcommand{\ganttcharttable}[9]{
    \newtoks \days

    \days{}     % Initializing

    \def \titledimension{#2} % Getting the height and width of the title
    \pgfmathsetmacro \titleheight{{\titledimension}[0]}
    \pgfmathsetmacro \titlewidth{{\titledimension}[1]}
    
    \def \startdate{#5}
    \def \enddate{#6}
    \def \leavecount{#8}

    \def \leavedays{{#9}}

    \def \fontset{\scriptsize} % Setting the title and label font size


    %   Displaying the day names with color
    \def\pgfcalendarweekdayletter##1{%
        \fontset%        To change the weekday font size
        \ifcase##1Mon \or Tue \or Wed \or Thr \or Fri \or Sat \or \textcolor{red}{Sun}\fi%
    }

    %  Using internal macros -- temporarily redefine the behavior.
    \makeatletter
    \ganttset{
        conceptName/.code={ % Writing custom code
            \pgfqkeysalso{/pgfgantt}{@conceptName={##1}} % Setting the custom values
        },
        @conceptName/.code args={##1}{
            \pgfqkeysalso{/pgfgantt}{progress={100},progress label text={##1}}   % Make the progress to 100% for all tasks with labels
        }
    }
    \makeatother    % Make it as a custom macro

    % Getting Leave Days
    \foreach \i in {0,...,\inteval{\leavecount - 1}} {
        \pgfmathsetmacro \leaveday{\leavedays[\i][0]}
        \pgfmathsetmacro \leavedayname{\leavedays[\i][1]}
        \global\days\expandafter{%
            \expanded{%
                \the\days \noexpand\verticalrule{\leaveday}{\leavedayname}%
            }%
        }%
    }


    \begin{ganttchart}[
        vgrid = {*{1}{gray!30, dashed}},    % Vertical grid style
        % expand chart=0.5\textwidth, % Expanding the based on the paper
        title height=#1, % Must be less than or eqaul to 1
        title label font=\fontset,
        bar height=#3, 
        bar/.style={
             fill=#4    % blue!60
        },
        x unit=\titlewidth mm,   % Width of the individual cells
        y unit title=\titleheight mm, % Height of the individual cells
        time slot format=little-endian,     % Defining the time format used
        bar label node/.append style={
            font=\fontset,
        },
        inline,     % For displaying the labels on the bars
        bar inline label node/.style={
            font=\tiny,
            color=white,
        },
        progress label text={},     % Dummy space for setting the concept names
        bar progress label font=\fontset,   % Changing progress bar label font size
        labelposLeft/.style={
            bar progress label node/.append style={
                anchor=west, 
                left=4pt
            }, 
            bar progress label anchor=west,
        },   % Adjusting the label position of the right most labels
        vrule/.append style={red!30, thin},
        vrule label node/.style={
            anchor=north,
            font=\fontset,
            rotate=90,
            xshift=-16,
            yshift=-2
        }
    ]{\startdate}{\enddate}
        \gantttitlecalendar{
            month=name,
            day,
            weekday=letter,
        } \\
        
       #7
       \the\days
    \end{ganttchart}
    
    \renewcommand{\days}{{ }}
}

\newcommand{\verticalrule}[2]{
    \ganttvrule{}{#1}
    \ganttvrule[vrule offset=-0.001]{#2}{#1}
}

\begin{document}

%   #1 -- Height of the titles &lt;= 1
%   #2 -- Height and Width of the individual cells in mm
%   #3 -- Height of the bars
%   #4 -- Color of the bars
%   #5 -- Plan start date in the format like DD.MM.YYYY
%   #6 -- Plan end date in the format like DD.MM.YYYY
%   #7 -- concept name, no.of days, start date and end date
%   #8 -- Leave Day Count including Sundays
%   #9 -- Leave Days


\ganttcharttable
    {0.9}
    {8,6}
    {0.5}
    {blue!60}
    {11.4.2024}
    {11.5.2024}
    {
        \ganttbar[conceptName=Knowing on numbers]{1 Day}{11.4.2024}{11.4.2024} \\
        \ganttbar[conceptName=Algebric Expressions]{6 Days}{13.4.2024}{18.4.2024} \\
        \ganttbar[conceptName=Operation on numbers]{3 Days}{19.4.2024}{21.4.2024} \\
        \ganttbar[conceptName=Operation on decimals]{3 Days}{22.4.2024}{24.4.2024} \\ 
        \ganttbar[conceptName=Area and Perimeter]{5 Days}{25.4.2024}{29.4.2024} \\
        \ganttbar[conceptName=Triangles, labelposLeft]{6 Days}{30.4.2024}{5.5.2024}
        \ganttbar[]{4 Days}{8.5.2024}{11.5.2024}
    }
    {2}
    {
        {"20.4.2024", "Leave"},
        {"10.5.2024", "Holiday"}
    }


\end{document}</code></pre>
<p id="bkmrk-%C2%A0-9"></p>
<h2 id="bkmrk-parameters-used"><span style="text-decoration: underline;"><strong>Parameters Used</strong></span></h2>
<p id="bkmrk-%231----height-of-the-" style="text-align: justify;"><strong>#1 -- Height of the titles &lt;= 1 - </strong>The distance between the titles row cells need to be less that or equal to 1<br><strong>#2 -- Height and width of the individual cells in mm</strong><br><strong>#3 -- Height of the bars</strong><br><strong>#4 -- Color of the bars</strong><br><strong>#5 -- Plan start date in the format like DD.MM.YYYY</strong><br><strong>#6 -- Plan end date in the format like DD.MM.YYYY</strong><br><strong>#7 -- concept name, no. of days, start date and end date - </strong>Passing the data in the format like \ganttbar [conceptName=&lt;Name of the concept&gt;] {&lt;Day difference&gt;} {&lt;Start date&gt;} {&lt;End Date&gt;} \\<br><strong>#8 -- Leave Day Count, including Sundays</strong><br><strong>#9 -- Leave Days with names - </strong>Passing the date to be leave like { {&lt;date&gt;, &lt;name&gt;}, {&lt;date&gt;, &lt;name&gt;} }</p>
<p id="bkmrk-%C2%A0-10"></p>
<h2 id="bkmrk-output-of-the-latex-"><span style="text-decoration: underline;"><strong>Output of the LaTeX Code</strong></span></h2>
<p id="bkmrk--4"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/Qp3iolVOhFb8tG1p-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/Qp3iolVOhFb8tG1p-image.png" alt="image.png" width="533" height="275"></a></p>
<p id="bkmrk-%C2%A0-11"></p>
<h2 id="bkmrk-challenges"><span style="text-decoration: underline;"><strong>Challenges</strong></span></h2>
<ul id="bkmrk-for-one-day-tasks%2C-t">
<li class="null" style="text-align: justify;">For one-day tasks, the labels are not able to fit properly inside the task bars.</li>
<li class="null" style="text-align: justify;">The labels of the bars overlap when the same day has different tasks.</li>
<li class="null" style="text-align: justify;">It is impossible to remove the weekend days from the calendar title in the chart.</li>
<li class="null" style="text-align: justify;">Efforts were put into adjusting the bar labels on the rightmost side of the Gantt chart.</li>
<li class="null" style="text-align: justify;">Can't be able to individually modify the weekday titles.</li>
<li class="null" style="text-align: justify;">It is difficult to move the leave lines behind the bars and labels.</li>
</ul>
<p id="bkmrk-%C2%A0-12"></p>