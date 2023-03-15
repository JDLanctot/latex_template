# LaTex Scientific Writing Template

This LaTex template is designed to speed up scientific writing by structuring the content in a similar file structure as HTML website design. This makes it easier to organize your writing and quickly navigate through your document.

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

#### Sections and Subsections

The document structure is organized using sections and subsections. Each section and subsection has a corresponding file in the `sections` folder. To add a new section or subsection, simply create a new `.tex` file in the `sections` folder and add it to the `main.tex` file using the `\input{sections/<filename>}` command.

#### Figures and Tables

Figures and tables can be easily added to the document using the `\includegraphics{<filename>}` and `\begin{table}` commands, respectively. You can also add captions to your figures and tables using the `\caption{<caption>}` command. Some examples are left in the document to guide you in filling out the required information.

#### References

The references is automatically generated using BibTeX. You can add your references to the `reference.bib` file and cite them in your document using the `\cite{<key>}` command. Note that you will not see citations appear in the references section until you have actually cited them in the document -- at which point they will be dynamically added in the correct order.

### Customization

The `hightlight.sty` file allows for assigning colors to table values based on how large the values are relative to a minimum and maximum value -- thereby giving a gradient which allows for added vizualization of the table contents. All of the additional styling can be found in the `nature.tex` file which makes seeks to style things like Nature publications. The majority of this file was created and shared on the internet by Peter Czoschke, in 2004.

## Contributing

If you have any suggestions or improvements for this template, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
