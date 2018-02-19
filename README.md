# Bylaws for the Gainesville Hackerspace
The current bylaws for the Gainesville Hackerspace.

## LaTeX installation
### Linux: 
In ubuntu Karmic, the following packages are sufficient to successfully make
this document.

`tex texlive-latex3 texlive-latex-extra`

Fewer may be sufficient.

### How to work with Windows
1. Download the [TexLive Installer](https://www.tug.org/texlive/acquire-netinstall.html) (look for the install-tl-windows.exe)
1. Start the installer, and choose "Custom" mode.
1. Under the `Collections` section, select the following:
    * Essential programs and files
    * US and UK English
    * LaTeX fundamental packages
    * LaTeX additional packages
    * Windows-only support programs
1. Use `latexmk` (installed by TexLive) to compile the LaTeX:
    1. Open a command prompt and navigate to this directory
    1. Run `latexmk -pdf` to compile and generate the pdf documents.
        * If `latexmk` cannot be found (its not in your Windows path), you can either add the bin\ directory under where you installed the TexLive packages, or do a fully-qualified path to that exe: ie, `C:\texlive\2017\bin\latexmk.exe -pdf`

Consider using `vscode` (text editor) and the `Latex Workshop` (vscode extension) to make your life easier. It will automatically recompile the .tex documents on save, and show you live previews of the pdf while you are writing.