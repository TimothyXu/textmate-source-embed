# TextMate Source Embedding
Allows TextMate to recognise source code embedded in text markups like HTML, MultiMarkDown, Pandoc, Markdown and etc. so that syntax highlighting and other features can be achieved.

##Usage

* Download ZIP
* Open source-embed.tmbundle to install
* Open Bundle Editor in TextMate (Control+Option+Command+B)
* Navigate to the markup formats that you would like to use this bundle in, i.e. HTML, Markdown, Pandoc, etc.
* Navigate to Language Grammars and edit the file
* Insert the following line `{	include = 'meta.embed'; },` immediately after the first `patterns = (`. (See screen shot, line 12 inserted)

![HTML](images/HTML.png)

* Embed source code in your text documents by writing in the following syntax, **without** the two backticks (\\): (See screen shot)
```
\~~~{.python}

#Example code
def test(): pass

\~~~
```
![Example Code](images/code.png)

* You can easily add another source language by editing the Language Grammar file of _this_ bundle, named Source Embedding. It should be self-explanatory. (See screen shot)
![Language Grammar](/images/grammar.png)

##Clarification

This bundle only makes _TextMate_ recognise source code in your text markups, it will not make such source code to be recognised and rendered correctly by your HTML/Markup parsers. HOWEVER, the brilliant utility [Pandoc](http://johnmacfarlane.net/pandoc/index.html) (and also GitHub's own markup parser) recognises the syntax used by this bundle and will render your code correctly and can output via LaTeX, HTML, EPUB, docx, and so on. This is especially convenient when combined with the [Pandoc TextMate Bundle](https://github.com/dsanson/Pandoc.tmbundle).

##Licence
Credit is due to [Nick Dunn's excellent post](https://developmentality.wordpress.com/2011/03/23/pandoc-an-essential-tool-for-markdown-users/) which gave me the idea for this bundle. 

Copyright (C) 2015 Timothy Xu  
  
This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.  
  
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

The full GNU GPL 3 licence can be found in LICENCE.

##Contributing
All contributions are welcomed.
