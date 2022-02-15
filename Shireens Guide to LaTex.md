## Shireen's Guide to LaTex for Jupyter Notebook

[**LaTex**](https://www.latex-project.org/about/) (pronounced LAH-tech or LAY-tech) is a document preparation sytem used for typesetting. Jupyter Notebook supports the use of LaTex in markdown cells. LaTex is great for easily adding nicely-formatted math equations to your notebooks.

### Adding LaTex to a Jupyter Notebook Markdown Cell


* For **inline** LaTex code, just add a dollar sign `$` before and after the code. Make sure there's a space between the `$` and the code. For example, if you want to write 
"Add $ \frac{2}{3} $ cups flour," type `Add $ \frac{2}{3} $ cups flour` into your markdown cell.


* For **display** mode, which gives your code its own centered paragraph, use two dollar signs `$$` instead of one. For example, if you want to write: $$ \mu = \frac{\Sigma\ X_{i}}{N} $$ <br /> you should surround the code with two dollar signs and a space on each side, like this: `$$ \mu = \frac{\Sigma\ X_{i}}{N} $$`

### Formatting
* A single backslash `\` adds a space
* Two backslashes `\\` adds a new line
* $ A^{superscript} $ is added in braces like so: `^{}`. For example, if you want to write $ 9^{10-2} $, you type `$ 9^{10-2} $`.
* $ A_{subscript} $ is added with `_{}`. So if you want to display $ X_{i} $, you type `$  X_{i} $`.
* You can add roots by typing `$ \sqrt[index]{radicand} $`. So if you want to display $ \sqrt[3]{27} $, type `$ \sqrt[3]{27} $`.
* To display a fraction, type `$ \frac{numerator}{denominator} $ `. Example: if you want to display $ \frac{5x}{3y} $, type `$ \frac{5x}{3y} $`
* to add Greek letters, mathematial symbols, and other special characters supported by LaTex, use a backslash `\` followed by LaTex's name for the symbol. For example, to display $ \gamma $, type `$ \gamma $`. If you want the uppercase version of a Greek letter, make the first character after the backslash uppercase. So `$ \Gamma $` becomes $ \Gamma $.
* A good reference guide for learing more about LaTex, by Khelifi Ahmed Aziz: [Learn How to Write Markdown & LaTeX in The Jupyter Notebook](https://towardsdatascience.com/write-markdown-latex-in-the-jupyter-notebook-10985edb91fd)

The End!
