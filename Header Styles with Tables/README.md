<h1 id="bkmrk-list-of-headers"><span style="color: rgb(230, 126, 35); background-color: rgb(194, 224, 244);"><strong>List of Headers</strong></span></h1>
<p id="bkmrk-%C2%A0"></p>
<h2 id="bkmrk-latex-link"><span style="text-decoration: underline;"><strong>LaTeX Link</strong></span></h2>
<h3 id="bkmrk-lapis-report---%3E-hea" style="padding-left: 40px;">Intern Works --&gt; Header --&gt; 1 Line Header.tex</h3>
<h3 id="bkmrk-lapis-report---%3E-hea-1" style="padding-left: 40px;">Intern Works --&gt; Header --&gt; 2 Lines Header.tex</h3>
<h3 id="bkmrk-lapis-report---%3E-hea-2" style="padding-left: 40px;">Intern Works --&gt; Header --&gt; 3 Lines Header.tex</h3>
<p id="bkmrk-%C2%A0-1"></p>
<p id="bkmrk-%C2%A0-2"></p>
<h2 id="bkmrk-1-row"><span style="text-decoration: underline;"><strong>One Line Header</strong></span><br></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=2cm,bottom=2.5cm,left=0.5cm,right=0.5cm}
\usepackage{lipsum}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{ragged2e}
\usepackage{xcolor}
\usepackage{setspace}
\usepackage{array}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\def \schoolname{ABC School}

% #1 -- Heading name
% #2 -- Class

\newcommand{\headeroneline}[2]{
  \fancypagestyle{pagehf}{
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \fancyhead{ }
    \fancyfoot{ }
    
    \fancyfoot[L]{\textcolor{black}{Learn Basics}}%
    \fancyfoot[C]{\textcolor{black}{\thepage}}%
    \fancyfoot[R]{\textcolor{black}{Class #2 | \schoolname}}%
    
    \fancyhead[L]{%
        \includegraphics[width=2.5cm]{img/logo.png}\\%
        www.learnbasics.fun%
    }
    \fancyhead[C]{%
        \renewcommand{\arraystretch}{1.5}
        \begin{tabular}{@{}c}
            \huge{\textbf{#1}}%
        \end{tabular} \smallskip
    }

     \fancyhead[R]{}

    \renewcommand{\headrulewidth}{1.2pt}
    \renewcommand{\footrulewidth}{1.2pt}
    \renewcommand{\headrule}{\color{blue!70}\hrulefill}
     \renewcommand{\footrule}{\color{blue!70}\hrulefill}
 }
 \pagestyle{pagehf}
}

\begin{document}
\headeroneline{Header and Footer Styling}{7}
\setlength{\headsep}{2cm}
\lipsum[6]

\end{document}</code></pre>
<h3 id="bkmrk-output"><span style="text-decoration: underline;"><strong>Output</strong></span></h3>
<p id="bkmrk-"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/OSk4c2gwF9xNmLJV-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/OSk4c2gwF9xNmLJV-image.png" alt="image.png"></a></p>
<p id="bkmrk--1"></p>
<h2 id="bkmrk-2-rows"><span style="text-decoration: underline;"><strong>Two Lines Header</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%5D"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=2cm,bottom=2.3cm,left=0.5cm,right=0.5cm}
\usepackage{lipsum}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{ragged2e}
\usepackage{xcolor}
\usepackage{setspace}
\usepackage{array}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\def \schoolname{ABC School}

% #1 -- Heading name
% #2 -- Class

\newcommand{\headertwolines}[2]{
  \fancypagestyle{pagehf}{
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \fancyhead{ }
    \fancyfoot{ }

    \fancyfoot[L]{\textcolor{black}{Learn Basics}}%
    \fancyfoot[C]{\textcolor{black}{\thepage}}%
    \fancyfoot[R]{\textcolor{black}{Class #2 | \schoolname}}%
    
    \fancyhead[L]{%
        \includegraphics[width=2.5cm]{img/logo.png}\\%
        www.learnbasics.fun \vspace{0.1cm}%
    }
    \fancyhead[C]{
        \begin{tabular}{@{}c}
            \huge{\textbf{\schoolname}} \\ \\
            \Large{#1}
        \end{tabular} \smallskip
    }

     \fancyhead[R]{}

    \renewcommand{\headrulewidth}{1.2pt}
    \renewcommand{\footrulewidth}{0pt}
    \renewcommand{\headrule}{\color{blue!70}\hrulefill}
    \renewcommand{\footrule}{\color{blue!70}\hrulefill}
    
  }
  \pagestyle{pagehf}
}


\begin{document}

\headertwolines{Header and Footer Styles}{6}
\setlength{\headsep}{2cm}
\lipsum[6]


\end{document}</code></pre>
<h3 id="bkmrk-output-1"><span style="text-decoration: underline;"><strong>Output</strong></span></h3>
<p id="bkmrk--2"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/A2NZXITiiN2wNr3n-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/A2NZXITiiN2wNr3n-image.png" alt="image.png"></a></p>
<p id="bkmrk-%C2%A0-3"></p>
<h2 id="bkmrk-two-line-header-with"><span style="text-decoration: underline;"><strong>Two Line Header with Rule</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C-1"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=2cm,bottom=2.3cm,left=0.5cm,right=0.5cm}
\usepackage{lipsum}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{ragged2e}
\usepackage{xcolor}
\usepackage{setspace}
\usepackage{array}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\def \schoolname{ABC School}

\newcommand{\headertwolineswithrule}[1]{
    \fancypagestyle{pagehf}{
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \fancyhead{ }
    \fancyfoot{ }
    \fancyhead[L]{
        \includegraphics[width=2.5cm]{img/logo.png}\\
        www.learnbasics.fun
        \vspace{-0.8cm}
    }
    \fancyhead[C]{
        \begin{tabular}{@{}c}%
            \huge{\textbf{#1}} \\ 
            \rule{300pt}{1pt}\\
            \Large{\schoolname}%
        \end{tabular}% 
    }%
    \fancyhead[R]{%
    
    }%
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \renewcommand{\headrule}{}
    \renewcommand{\footrule}{}
    }
    \pagestyle{pagehf}
    \setlength{\headsep}{2cm}
}

\begin{document}

\headertwolineswithrule{Header and Footer Styles}
\lipsum[5]


\end{document}</code></pre>
<h3 id="bkmrk-%C2%A0-4"></h3>
<h3 id="bkmrk-output-2"><span style="text-decoration: underline;"><strong>Output</strong></span></h3>
<p id="bkmrk--3"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/IHoJnaAJytp1ZMiY-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/IHoJnaAJytp1ZMiY-image.png" alt="image.png" width="468" height="147"></a></p>
<p id="bkmrk-%C2%A0-5"></p>
<h2 id="bkmrk-2-rows-with-table"><span style="text-decoration: underline;"><strong>Two Lines Header with Table</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C-2"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=2cm,bottom=2.3cm,left=0.5cm,right=0.5cm}
\usepackage{lipsum}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{ragged2e}
\usepackage{xcolor}
\usepackage{setspace}
\usepackage{array}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\def \schoolname{ABC School}


% #1 -- Heading name
% #2 -- Class
% #3 -- Subject
% #4 -- Track name


\newcommand{\headerWithTwoCols}[4]{
  \fancypagestyle{pagehf}{
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \fancyhead{ }
    \fancyfoot{ }

    \fancyfoot[L]{\textcolor{black}{Learn Basics}}%
    \fancyfoot[C]{\textcolor{black}{\thepage}}%
    \fancyfoot[R]{\textcolor{black}{Class #2 | \schoolname}}%
    
    \fancyhead[L]{
        \includegraphics[width=2.5cm]{img/logo.png}\\
        www.learnbasics.fun
        \vspace{-0.2cm} \\
    }
    \fancyhead[C]{
        \begin{tabular}{@{}c}%
            \huge{\textbf{#1}} \\ \smallskip% 
            \rule{300pt}{1pt}\\
            \Large{\schoolname}%
        \end{tabular} \vspace{0.1cm}% 
    }%
    \fancyhead[R]{ \renewcommand{\arraystretch}{1.5}%
        \begin{tabular}{|&gt;{\centering\arraybackslash}m{1.5cm}|&gt;{\centering\arraybackslash}m{1.5cm}|}%
            \hline%
            \multicolumn{2}{|c|}{\textbf{\Large #3}} \\%
            \hline%
            Class #2 &amp; #4  \\
            \hline%
        \end{tabular}%
        \vspace{0.1cm}%
    }%
    \renewcommand{\headrulewidth}{1.2pt}
    \renewcommand{\footrulewidth}{0pt}
    \renewcommand{\headrule}{\color{blue!70}\hrulefill}
    \renewcommand{\footrule}{\color{blue!70}\hrulefill}
 }
 \pagestyle{pagehf}
}

% #1 -- Heading name
% #2 -- Class
% #3 -- Section
% #4 -- Subject
% #5 -- Track name
% #6 -- Student count

\newcommand{\headerWithThreeCols}[6]{
  \fancypagestyle{pagehf}{
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \fancyhead{ }
    \fancyfoot{ }

    \fancyfoot[L]{\textcolor{black}{Learn Basics}}%
    \fancyfoot[C]{\textcolor{black}{\thepage}}%
    \fancyfoot[R]{\textcolor{black}{Class #2 | \schoolname}}%
    
    \fancyhead[L]{
        \includegraphics[width=2.5cm]{img/logo.png}\\
        www.learnbasics.fun
        \vspace{0.2cm}%
    }
    \fancyhead[C]{
        \begin{tabular}{@{}c}%
            \huge{\textbf{#1}} \\ \smallskip%
            \rule{300pt}{1pt}\\
            \Large{\schoolname}%
        \end{tabular} \vspace{0.2cm}% 
    }%
    \fancyhead[R]{ \renewcommand{\arraystretch}{1.3}%
        \begin{tabular}{|&gt;{\centering\arraybackslash}m{1.5cm}|&gt;{\centering\arraybackslash}m{1.5cm}|}%
            \hline%
            \multicolumn{2}{|c|}{\textbf{\Large #4}} \\%
            \hline%
            Class #2 &amp; #5  \\
            \hline%
            #3 &amp; #6 \\
            \hline%
        \end{tabular} \vspace{0.1cm}%
    }%
    
    \renewcommand{\headrulewidth}{1.2pt}
    \renewcommand{\footrulewidth}{0pt}
    \renewcommand{\headrule}{\color{blue!70}\hrulefill}
    \renewcommand{\footrule}{\color{blue!70}\hrulefill}
 }
 \pagestyle{pagehf}
 \setlength{\headsep}{2cm}
}

\begin{document}

\headerWithTwoCols
    {Header and Footer Styling}
    {6}
    {Science}
    {Track 1}


\lipsum[4-6]

\newpage

\headerWithThreeCols
    {Header and Footer Styling}
    {6}
    {A}
    {Science}
    {Track 2}
    {45}

\vspace*{0.3cm}

\lipsum[4-9]

\end{document}</code></pre>
<h3 id="bkmrk--4"></h3>
<h3 id="bkmrk-output-3"><span style="text-decoration: underline;"><strong>Output</strong></span><br></h3>
<p id="bkmrk--5"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/YC7XT0bEgNNz8eqD-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/YC7XT0bEgNNz8eqD-image.png" alt="image.png"></a></p>
<p id="bkmrk--6"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/gAv5EwqfJdJdHHSq-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/gAv5EwqfJdJdHHSq-image.png" alt="image.png" width="630" height="114"></a></p>
<p id="bkmrk--7"></p>
<h2 id="bkmrk-3-rows"><span style="text-decoration: underline;"><strong>Three Lines Header</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C-3"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=2cm,bottom=2.5cm,left=0.5cm,right=0.5cm}
\usepackage{lipsum}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{ragged2e}
\usepackage{xcolor}
\usepackage{setspace}
\usepackage{array}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\def \schoolname{ABC School }


% #1 -- Heading name
% #2 -- Class

\newcommand{\headerthreelinescenter}[2]{
  \fancypagestyle{pagehf}{
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \fancyhead{ }
    \fancyfoot{ }

    \fancyfoot[L]{\textcolor{black}{Learn Basics}}%
    \fancyfoot[C]{\textcolor{black}{\thepage}}%
    \fancyfoot[R]{\textcolor{black}{Class #2 | \schoolname}}%
    
    \fancyhead[L]{%
        \includegraphics[width=2.5cm]{img/logo.png}\\%
        www.learnbasics.fun \\% % After this one space is needed
    }
    \fancyhead[C]{%
        \renewcommand{\arraystretch}{1.5}
        \begin{tabular}{@{}c}
            \huge{\textbf{\schoolname}} \\
            \Large{#1} \\
            \large{Class - #2}%
        \end{tabular} \smallskip%
        %\hspace*{6cm}%
    }%

     \fancyhead[R]{}

    \renewcommand{\headrulewidth}{1.2pt}
    \renewcommand{\footrulewidth}{0pt}
    \renewcommand{\headrule}{\color{blue!70}\hrulefill}
    \renewcommand{\footrule}{\color{blue!70}\hrulefill}
    
  }
  \pagestyle{pagehf}
  \vspace*{1cm}
}

\begin{document}

\headerthreelinescenter{Header and Footer Styling - With large text happened}{7 A}
\setlength{\headsep}{2cm}

\lipsum[6]

\end{document}</code></pre>
<h3 id="bkmrk-output-4"><span style="text-decoration: underline;"><strong>Output</strong></span></h3>
<p id="bkmrk--8"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/7sA5BCX1sR3fZuJ6-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/7sA5BCX1sR3fZuJ6-image.png" alt="image.png"></a></p>
<p id="bkmrk--9"></p>
<h2 id="bkmrk-with-chapter-name"><span style="text-decoration: underline;"><strong>Three Lines Header Left Aligned</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%5D-1"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=2cm,bottom=2.5cm,left=0.5cm,right=0.5cm}
\usepackage{lipsum}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{ragged2e}
\usepackage{xcolor}
\usepackage{setspace}
\usepackage{array}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\def \schoolname{ABC School }

% #1 -- Heading name
% #2 -- Class

\newcommand{\headerthreelinesleft}[2]{
  \fancypagestyle{pagehf}{
    \renewcommand{\headrulewidth}{0pt}
    \renewcommand{\footrulewidth}{0pt}
    \fancyhead{ }
    \fancyfoot{ }

    \fancyfoot[L]{\textcolor{black}{Learn Basics}}%
    \fancyfoot[C]{\textcolor{black}{\thepage}}%
    \fancyfoot[R]{\textcolor{black}{Class #2 | \schoolname}}%
    
    \fancyhead[L]{%
        \includegraphics[width=2.5cm]{img/logo.png}\\%
        www.learnbasics.fun \\% % After this one space is needed
    }
    \fancyhead[C]{%
        \renewcommand{\arraystretch}{1.5}
        \begin{tabular}{@{}|l}
            \huge{\textbf{\schoolname}} \\
            \Large{#1} \\
            \large{Class - #2}%
        \end{tabular} \smallskip%
        %\hspace*{6cm}%
    }%

     \fancyhead[R]{}

    \renewcommand{\headrulewidth}{1.2pt}
    \renewcommand{\footrulewidth}{0pt}
    \renewcommand{\headrule}{\color{blue!70}\hrulefill}
    \renewcommand{\footrule}{\color{blue!70}\hrulefill}
    
  }
  \pagestyle{pagehf}
  \vspace*{1cm}
}



\begin{document}

\headerthreelinesleft{Header and Footer Styling - With large text happened}{7 A}
\setlength{\headsep}{2cm}

\lipsum[6]

\end{document}</code></pre>
<h3 id="bkmrk-output-5"><span style="text-decoration: underline;"><strong>Output</strong></span><br></h3>
<p id="bkmrk--10"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/XC5FFZ6FjaKsFqf0-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/XC5FFZ6FjaKsFqf0-image.png" alt="image.png"></a></p>
<p id="bkmrk-%C2%A0-6"></p>
<h2 id="bkmrk-three-line-header-wi"><span style="text-decoration: underline;"><strong>Three Line Header With Chapter Name</strong></span></h2>
<pre id="bkmrk-%5Cdocumentclass%5B11pt%2C-4"><code class="language-latex">\documentclass[11pt, a4paper]{article}
\usepackage{geometry}
\geometry{top=2cm,bottom=2.5cm,left=0.5cm,right=0.5cm}
\usepackage{lipsum}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{ragged2e}
\usepackage{xcolor}
\usepackage{setspace}
\usepackage{array}
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}

\def \schoolname{ABC School }


% #1 -- Class
% #2 -- Subject
% #3 -- Teacher name
% #4 -- Chapter name

\newcommand{\headerthreelinesdiff}[4]{
    \fancypagestyle{pagehf}{%
        \renewcommand{\headrulewidth}{0pt}%
        \renewcommand{\footrulewidth}{0pt}%
        \fancyhead{%
        }%
        \fancyfoot{%
        }%
        \renewcommand{\footrulewidth}{1pt}%
        \fancyfoot[L]{%
            \vspace{0.5cm}%
            \textcolor{black}{Learn Basics}%
        }%
        \fancyfoot[C]{%
            \vspace{0.5cm}%
            \textcolor{black}{\thepage}%
        }%
        \fancyfoot[R]{%
            \vspace{0.5cm}%
            \textcolor{black}{#3 | #2 {-} DCP}%
        }%
        \fancyhead[L]{%
            \includegraphics[width=2.5cm]{img/logo.png}\\%
            www.learnbasics.fun \\ \vspace{1.2cm}
        }%
        \fancyhead[C]{%
            \Large \textbf{\schoolname - Learn Basics}\\%
            \vspace{0.2cm}%
            \Large \textbf{#2 Daily Chapter Planner}\\%
            \normalsize \rule{480pt}{1pt} Class #1\\%
            \Large\textbf{#4} \\%
        }%

        \renewcommand{\headrule}{}
        \renewcommand{\footrule}{\hrulefill}
        \renewcommand{\headrulewidth}{0pt}
        \renewcommand{\footrulewidth}{1.2pt}
    }%
    \pagestyle{pagehf}
    \vspace*{1cm}
}

\begin{document}

\headerthreelinesdiff{6}{Math}{Mr.Teacher}{1. Knowing Our Numbers}
\lipsum[6]

\end{document}</code></pre>
<h3 id="bkmrk-output-6"><span style="text-decoration: underline;"><strong>Output</strong></span></h3>
<p id="bkmrk--11"><a href="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/BJHXdf5ZrZiugYcF-image.png" target="_blank" rel="noopener"><img src="https://docs.learnbasics.fun/uploads/images/gallery/2024-04/scaled-1680-/BJHXdf5ZrZiugYcF-image.png" alt="image.png" width="589" height="202"></a></p>