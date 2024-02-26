# Dynamic Adjusting Line Graph

    This LaTeX line graph adjusts (or add more or add less) the xticks and yticks based on the user inputs. It can make it possible to include multiple plot lines in a single graph.


## Modification abilities:
It provides the ability to modify the


**1. xticks labels and yticks labels:**

       By default, it shows the numeric values.

You can change the xticks and yticks labels by passing the required labels as a 3rd and 4th parameters of the \linegraph command, respectively.


**2. Height and Width of the graph layout**

       Must pass the height and width in cm (Eg: 10cm, 13cm)

Changing the height and width of the graph layout is possible, Be careful when you change the width. If the label of the graph is not visible, then reduce the width.


**3. X-axis label styles**

       By default, it aligned at 45 degree.

You can't change the style of the X-axis label by passing the parameters in the \linegraph; whenever you want to change the angle, make some changes in the 'x label style part'.


**4. Line color of the graph**

It is possible to create or define your own color by edit the custom color declaration section in the code snippet,

<u>Syntax for declaring a custom color:</u>

     \definecolor{<your_command_name>}{RGB}{<color_rgb_value>}

        where,
        <your_command_name>, must be start with rgbColor and end with a number


**5. Extending the coordinates upto 12**

    Above 12 plots, you must adjust the height and width of the graph

- You can add upto 12 xticks and yticks by simply passing the parameters.
- Also, you can adjust the graph size using the enlarge x limits and enlarge y limits.
- The enlarge x limits must be negative.


**6. Graph outer axis color**

    By changing the color to any other color except white, you can make the graph line visible.

Change the value of the 'draw' in the code snippet to any other color.



## Custom Line Graph Command:

**Syntax:**

```tex
\linegraph{ <Height and Width } { <Y axis limits> } { <X-tick labels> } { <Y-tick labels> } { <X-Axis label> } { <Y-Axis Label> }{ <Graph Legends> } { <Array of Coordinates> } { <Graph Title> }
```

Where,

An Array of Coordinates is a collection of the number of graph lines, number of plots, and the coordinates of the lines.

Must pass the collection of the required array.

<u>Example:</u>

        {
                {2},   % No of Graph lines
                {10},    % No of plots
                {86,80,77,77,70,75,84,82,68,87},
                {81,84,80,90,88,82,76,74,64,69}   % Coordinates
        } 


## Screenshot:





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