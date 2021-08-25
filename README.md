<!-- Title -->
<div align="center">
    <h1><b>JITRI Beamer Template</b></h1>
</div>

<div align="center">
    <img class="aligncenter" src="images/template.jpg"/>
</div>
<br/>


<!-- Table of Contents -->
<p align="center">
    <a href="#what is it?">What is it?</a> •
    <a href="#for whom?">For Whom?</a> •
    <a href="#usage">Usage</a> •
    <a href="#tips">Tips</a>
</p>

<!-- Sections -->
## What is it?
This template is inspired and modified based on [XJTLU-Beamer-Template](https://github.com/yaoshanliang/XJTLU-Beamer-Template).


This project aims to create a template for presentation for the Jiangsu Industrial Technology Research Institute (JITRI). It was created a class called **jitri_format.cls** with a set of environments and commands related to the document. This template is not an official document from the JITRI. However, this template can be used to create classes, presentations, short courses, etc.

## For Whom?

This template can be useful for the JITRI researchers.

- <b>Researchers:</b> for presentations
  
- <b>Students:</b> for meeting, viva and dissertation defense

- <b>Employees:</b> for commercial presentations
## Usage

Copy or download the project.
  
- <b>Github:</b> https://github.com/ZHOUYI1023/JITRI-Latex-Beamer-Template
## Tips

Some tips for using this template

### Blocks

- Default Block
  
```tex
    \begin{block}{Default Block}
        Body of default block.
    \end{block}
```

- Alert Block
  
```tex
    \begin{alertblock}{Alert Block}
        Body of alert block.
    \end{alertblock}
```

- Example Block
  
```tex
    \begin{exampleblock}{Example Block}
        Body of example block.
    \end{exampleblock}
```

### Texts

- Example text
```tex
 \example{Text Example}
```

- Emphasis text
```tex
 \emph{Text emphasis}
```

### Boxes

- Simple Box

```tex
\simplebox{testando o simple box}
```

- Alert Box

```tex
\alertbox{testando o alert box}
```

- Success Box

```tex
\successbox{testando o success box}
```

### Videos

Use the `media9` package to include videos as 
```tex
\includemovie{width}{height}{videos/xxx.avi}
```

### Codes

It is possible to insert codes in this presentation. This template uses two packages for algorithms: `algorithm2e` and `listings`. 


- **Documentation** 
  
  - algorithm2e: [Algorithm2e Package Documentation](http://linorg.usp.br/CTAN/macros/latex/contrib/algorithm2e/doc/algorithm2e.pdf)
  
  - listings: [Listings Package Documentation](http://linorg.usp.br/CTAN/macros/latex/contrib/listings/listings.pdf)

The following example shows how to create a pseudocode:

```tex
\begin{algorithm}[H]
    \SetAlgoLined #includes indentation
    \LinesNumbered #includes lines number
    \SetKwInOut{Input}{input}
    \SetKwInOut{Output}{output}
    \Input{write the input}
    \Output{write the output}
    \KwData{write the data}
    \KwResult{Write the result}
    initialization\;
    \While{While condition}
    {
        instructions\;
        \eIf{condition}{
           instructions1\;
           instructions2\;
           }{
           instructions3\;
        }
    } 
    \caption{How to write algorithms}
\end{algorithm}
```

The following example shows how to insert a code that is in the project files:

```tex
\begin{frame}{Including Codes}
    \lstset{language=Python}
    \lstinputlisting[language=Python]{path_of_python_code.py}
\end{frame}
```

The following example shows how to insert a figure:

```tex
\begin{figure}
    \centering
    \caption{Caption of the Figure}
    \includegraphics[scale=1]{path_of_the_figure}
    \source{Source of the Figure}
    \label{fig:figlabel}
\end{figure}
```

The following example shows how to insert a multi-columns:

```tex
\begin{columns}{}
    \begin{column}{0.5\textwidth}
        \justify
        Text of the left side!
    \end{column}
    \begin{column}{0.5\textwidth}
        \justify
        Text of the right side!
    \end{column}
\end{columns}    
```

### Custom Commands

This template has some custom commands that are described below:

To put the department name
```tex
\department{Department Name}
```

To put the email
```tex
\email{user@domain}
```


