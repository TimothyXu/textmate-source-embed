# TextMate Source Embedding
Allows syntax highlighting and other features for source codes embedded in text documents like HTML, MultiMarkDown, Pandoc, Markdown, etc. in TextMate.

##Usage:

1. Download ZIP -->
2. Open Source_Embedding.tmbundle to install
3. Open Bundle Editor in TextMate (Control+Option+Command+B)
4. Navigate to the markup formats that you would like to use this bundle in, i.e. HTML, Markdown, Pandoc, etc.
5. Navigate to Language Grammars and edit the file
6. Insert the following line:

~~~{.source}

{	include = 'meta.embed'; },

~~~

immediately after the first

~~~{.source}

patterns = (
	
~~~  

7. Embed source code in your text documents by doing this:

\~~~{.python}

def test():
	pass

\~~~

8. You can easily add another source language by editing the Language Grammar file of _this_ bundle, named Source Embedding. It should be self-explanatory.

##License:
Please see LICENSE