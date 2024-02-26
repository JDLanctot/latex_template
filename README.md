This LaTex template is designed to speed up scientific writing by structuring the content in a similar file structure as HTML website design. This makes it easier to organize your writing and quickly navigate through your document.

FIND A SIMPLER VERSION [HERE](https://github.com/JDLanctot/latex_lab_report).

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
	- [Prerequisites](#prerequisites)
	- [Usage](#usage)
		- [Splitting and Compiling Files](#splitting-and-compiling-files)
		- [Document Structure](#document-structure)
		- [Text Formatting](#text-formatting)
		- [Equations and Mathematical Notation](#equations-and-mathematical-notation)
		- [Figures and Tables](#figures-and-tables)
		- [References](#references)
	- [Customization](#customization)
- [Academic Resources](#academic-resources)
	- [My Dotfiles](#my-dotfiles)
	- [Scholarship Applications](#scholarship-applications)
	- [Portfolio Website](#portfolio-website)
- [Contributing](#contributing)
- [License](#license)

## Features

- Structured content using nested sections and subsections
- Customizable table of contents with clickable links
- Easily add figures and tables with captions
- Automatically generated references
- Clean and professional looking document design

## Getting Started

To use this template, simply clone the repository or download the ZIP file and extract it to your computer. Open the `main.tex` file in your preferred LaTex editor and start writing your scientific paper!

### Prerequisites

To use this template, you will need a LaTex distribution installed on your computer, such as [TeX Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/), or upload the folder to your [Overleaf Accout](https://www.overleaf.com).

### Usage

The main file of the template is `main.tex`, which includes the `0-header.tex` file which imports all the necessary packages and commands. The structure is designed to allow subsections to be commented out from the `main.tex` to not render them to the compiled document. You can modify the content of the sections and subsections to match your writing needs. All of the files start with a number, or letter in the case of the preface content, to indicate the compiling sequence of the `main.tex` right from the folder structure.

#### Splitting and Compiling Files

The document structure is organized using sections to be drawn into the `main.tex` to keep organized. Each section has a corresponding file in the `sections` folder. To add a new section or subsection, simply create a new `.tex` file in the `sections` folder and add it to the `main.tex` file using the `\input{sections/<filename>}` command.

#### Document Structure

LaTeX documents are structured into sections, subsections, and chapters. The document class specifies the overall style and layout of the document. The `\section{}` command creates a new section, with automatic numbering and table of contents entry. The `\subsection{}` command creates a subsection, and so on for lower levels. Use the appropriate heading styles to create a clear hierarchy of sections and subsections. The page layout can be customized using the geometry package.

#### Text Formatting

LaTeX provides commands for formatting text, such as `\textbf{}` for bold, `\textit{}` for italic, `\underline{}` for underline, and `\fontsize{}{}` for changing the font size. Use these commands to create well-formatted and visually appealing documents. The font style and size can be set using the document class or the fontspec package. Avoid using manual formatting commands like `\vspace{}` and `\hspace{}` to create space between paragraphs and lines, use proper LaTeX environments instead. You can even use negative numbers in these commands to remove space.

#### Equations and Mathematical Notation

LaTeX is particularly well-suited for typesetting equations and mathematical notation. Use the `\begin{equation}` `\end{equation}` environment to create a numbered equation. Use the `\begin{align}` `\end{align}` environment to create a set of aligned equations, with one number for the entire set. Use the appropriate commands for mathematical symbols and operators, such as `\frac{}{}` for fractions, `\sqrt{}` for square roots, and `\int` for integrals. Use the `_` followed by a character of your choice to add subscripts and the `^` to add superscripts followed by a character of your choice. If you would like more than one character to be superscript or subscript, include them in `{}` directly after the `_` or `^`. Note that you can even use both of these modifiers, one after each other, if you need both a superscript and subscript on something. Use the amsmath package for additional mathematical commands and environments (already included in the `0-header.tex`).

#### Figures and Tables

LaTeX provides powerful tools for including figures and tables in documents. Figures and tables can be easily added to the document using the `\includegraphics{<filename>}` and `\begin{table}` commands, respectively. You can also add captions to your figures and tables using the `\caption{<caption>}` command and use the `\label{}` command to give the table a label which is used in the generation of the list of tables section in the preface. You can also use the \includegraphics[]{} command to insert an image file and apply the label and caption to these as well. Some examples are left in the document to guide you in filling out the required information.

#### References

The references is automatically generated using BibTeX. You can add your references to the `reference.bib` file and cite them in your document using the `\cite{<key>}` command. Note that you will not see citations appear in the references section until you have actually cited them in the document -- at which point they will be dynamically added in the correct order.

### Customization

The `hightlight.sty` file allows for assigning colors to table values based on how large the values are relative to a minimum and maximum value -- thereby giving a gradient which allows for added vizualization of the table contents. All of the additional styling can be found in the `nature.tex` file which makes seeks to style things like Nature publications. The majority of this file was created and shared on the internet by Peter Czoschke, in 2004.

## Academic Resources
Other GitHub repos to help you with Academic Success.

### My Dotfiles
Visit My Dotfiles repo for instructions and code to setup a Windows Computer for doing Scientific Research Coding: [My Dotfiles](https://github.com/JDLanctot/dotfiles). [[My Dotfiles]]

### Scholarship Applications
Visit my Scholarship Applications repo for instructions templates for applying to Graduate Level Scholarships, such as NSERC: [Scholarship Applications](https://github.com/JDLanctot/Scholarship-Applications). [[Scholarship Applications]]

### Portfolio Website
Visit Portfolio Website repo for instructions and code to an easy Portfolio Website and host it for FREE using GitHub: [Portfolio Website](https://github.com/JDLanctot/jdlanctot.github.io)). [[J.D.Lanctot's Portfolio]]

## Contributing

If you have any suggestions or improvements for this template, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details. [[LICENSE]]

