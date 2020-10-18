# Customizable template of Letter in LaTeX

## Description

**Customizable letter template**, `arthur-letter`, is classical with a **header**. The template allow **English conventions** (address and date at right and recipient information at left) and **french conventions** (address and date at left, and recipient information at right).

___

## Example preview

### English version

With respect to English conventions (without age, address and picture).

![English_cover_letter](https://github.com/ArthurBernard/Arthur-CV-LaTeX/blob/master/pictures/example_cover_letter_En.jpg)

___

### French version

With respect to French conventions (with picture, address and age).

![French_cover_letter](https://github.com/ArthurBernard/Arthur-CV-LaTeX/blob/master/pictures/example_cover_letter_Fr.jpg)

___

## Customized colors

The default theme color of letter is different kind of blue, but you can freely custom themes color, see below some non-exhaustive examples:

![Colored_Examples](https://github.com/ArthurBernard/Arthur-CV-LaTeX/blob/master/pictures/Colored_examples.jpg)

### Green

``` latex
\usepackage{xcolor}   
\definecolor{boxcolor}{HTML}{59762f}   
\definecolor{maincolor}{HTML}{556b2f}   
\definecolor{secondcolor}{HTML}{85b145}   
```

### Red

``` latex
\usepackage{xcolor}   
\definecolor{boxcolor}{HTML}{851919}   
\definecolor{maincolor}{HTML}{420c0c}   
\definecolor{secondcolor}{HTML}{861919}   
```

### Grey

``` latex
\usepackage{xcolor}   
\definecolor{boxcolor}{HTML}{606060}   
\definecolor{maincolor}{HTML}{484848}   
\definecolor{secondcolor}{HTML}{909090}   
```

### Yellow

``` latex
\usepackage{xcolor}   
\definecolor{boxcolor}{HTML}{bfa100}    
\definecolor{maincolor}{HTML}{5f5000}   
\definecolor{secondcolor}{HTML}{e1b400}    
```

___

## Letter environment style and commands

### Header

Set personal information (if you don't want to display one (or several) personal information let the command empty):

``` latex
\profilepic{path/picture}   
\letname{Your Name}   
\linkedin{/in/your-linkedin}   
\github{YourGitHub}   
\mail{your.address@email.com}   
\numberphone{your phone number}   
\lettitle{Title of your CV}   
\site{www.your-website.com}   
```

### Address and recipient

#### English convention

Address, date, and location are set at top right and the recipient is set at left.

``` latex
\address{John \capit{DOE},\\123, somestreet\\Somecity}   
\recipient{Sir \capit{COMPANY},\\456, somestreet\\Somecity}   
\location{Somecity, \today}   
```

#### French convention

Address, date and location are set at top left and the recipient is set at right.

``` latex
\addressfr{John \capit{DOE},\\123 rue des Avenue\\Ville}   
\recipientfr{Monsieur \capit{COMPANY},\\456 avenue des Rues\\Ville}   
\locationfr{Ville, \today}   
```

### Body

``` latex
\begin{letter}
  \subject{Example}
  \opening{Dear Sir or Madam,}
  % write here the letter body
  \closing{Your sincerly,} % To adapt following recipient
  \signing{John \capit{DOE}}
\end{coverletter}
```

___

## Requirements

- Compile with **XeLaTex** or **LuaLaTeX**.

- LaTeX packages:

  - fontspec;   
  - ClearSans;   
  - fontawesome;   
  - ragged2e;   
  - parskip;   
  - hyperref;   
  - textpos;   
  - titlesec;   
  - tikz;   
  - xcolor;   
  - multirow;   
  - xargs;   
  - tcolorbox;   
  - enumitem;   
  - ifthen.   

___

## MIT License

Copyright (c) 2019-2020 Arthur Bernard

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
