# TextMate Source Embedding
Allows TextMate to recognise source codes embedded in text markups like HTML, MultiMarkDown, Pandoc, Markdown and etc. so that syntax highlighting and other features can be achieved.

##Usage

* Download ZIP
* Open Source_Embedding.tmbundle to install
* Open Bundle Editor in TextMate (Control+Option+Command+B)
* Navigate to the markup formats that you would like to use this bundle in, i.e. HTML, Markdown, Pandoc, etc.
* Navigate to Language Grammars and edit the file
* Insert the following line: (See screen shot, line 12 inserted)

~~~{.source}

{	include = 'meta.embed'; },

~~~

immediately after the first

~~~{.source}

patterns = (
	
~~~  
![HTML](/Screen\ Shots/HTML.png)

* Embed source code in your text documents by writing in the following syntax, **without** the two backticks (\\): (See screen shot)
```
\~~~{.python}

#Example code
def test(): pass

\~~~
```
![Example Code](/Screen\ Shots/Code.png)

* You can easily add another source language by editing the Language Grammar file of _this_ bundle, named Source Embedding. It should be self-explanatory. (See screen shot)
![Language Grammar](/Screen\ Shots/Language\ Grammar.png)

##Clarification

This bundle only makes **TextMate** recognise source codes in your text markups, it will not make such source codes be recognised and rendered correctly by your HTML/Markup parsers. HOWEVER, the brilliant utility [Pandoc](http://johnmacfarlane.net/pandoc/index.html) (and also GitHub's own markup parser) recognises the syntax used by this bundle and will render your code correctly and can output via LaTeX, HTML, EPUB, docx, and so on. This is especially convenient when combined with the [Pandoc TextMate Bundle](https://github.com/dsanson/Pandoc.tmbundle).

##Licence
Please see LICENCE. Credit is due to [Nick Dunn's excellent post](https://developmentality.wordpress.com/2011/03/23/pandoc-an-essential-tool-for-markdown-users/) which gave me the idea for this bundle. 

##Contributing
All contributions welcomed.
