## Shireen's Guide to LaTex for Jupyter Notebook

[**LaTex**](https://www.latex-project.org/about/) (pronounced LAH-tech or LAY-tech) is a document preparation sytem used for typesetting. Jupyter Notebook supports the use of LaTex in markdown cells. LaTex is great for easily adding nicely-formatted math equations to your notebooks.

### Adding LaTex to a Jupyter Notebook Markdown Cell


* For **inline** LaTex code, just add a dollar sign `$` before and after the code. Make sure there's a space between the `$` and the code. For example, if you want to write "Add <img src="https://render.githubusercontent.com/render/math?math=\frac{2}{3} "> cups flour," type `Add $ \frac{2}{3} $ cups flour $` into your markdown cell.


* For **display** mode, which gives your code its own centered paragraph, use two dollar signs `$$` instead of one. For example, if you want to write:

<img align="center" src="https://render.githubusercontent.com/render/math?math=\mu = \frac{\Sigma\ X_{i}}{N}">


then you should type: `$$ \mu = \frac{\Sigma\ X_{i}}{N} $$`

**Note:** GitHub doesn't read LaTex in Markdown documents the same way Jupyter Notebooks does, so the "centered paragraph" above isn't actually centered the way it would be in a Jupyter Notebook.

### Formatting
* A single backslash `\` adds a space
* Two backslashes `\\` adds a new line
* <img src="https://render.githubusercontent.com/render/math?math=A^{superscript}"> is added in braces like so: `^{}`. For example, if you want to write <img src="https://render.githubusercontent.com/render/math?math=9^{10-2}">, you type `$ 9^{10-2} $`
* <img src="https://render.githubusercontent.com/render/math?math=A_{subscript}"> is added with `_{}`. So if you want to display <img src="https://render.githubusercontent.com/render/math?math=X_{i}">, you type `$  X_{i} $`
* You can add roots by typing `$ \sqrt[index]{radicand} $`. So if you want to display <img src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{27}">, type `$ \sqrt[3]{27} $`
* To display a fraction, type `$ \frac{numerator}{denominator} $ `. Example: if you want to display <img src="https://render.githubusercontent.com/render/math?math=\frac{5x}{3y}">\, type `$ \frac{5x}{3y} $`
* to add Greek letters, mathematial symbols, and other special characters supported by LaTex, use a backslash `\` followed by LaTex's name for the symbol. For example, to display <img src="https://render.githubusercontent.com/render/math?math=\gamma">, type `$ \gamma $`. If you want the uppercase version of a Greek letter, make the first character after the backslash uppercase. So `$ \Gamma $` becomes <img src="https://render.githubusercontent.com/render/math?math=\Gamma">

* A good reference guide for learing more about LaTex, by Khelifi Ahmed Aziz: [Learn How to Write Markdown & LaTeX in The Jupyter Notebook](https://towardsdatascience.com/write-markdown-latex-in-the-jupyter-notebook-10985edb91fd)

### Note:
If you want to save your Jupyter Notebook in Markdown format and share it on GitHub, you will need to make some adjustments before it will display correctly on GitHub. Wherevever you have LaTex code, you will need to remove the surrounding dollar signs and spaces, and paste the remaining code into this tag: `<img src="https://render.githubusercontent.com/render/math?math=LATEXCODE">`, where `LATEXCODE` gets replaced by your code. For example, if your original Markdown document says `$ \frac{5x}{3y} $`, that needs to be changed to `<img src="https://render.githubusercontent.com/render/math?math=\\frac{5x}{3y}">`

The End!
