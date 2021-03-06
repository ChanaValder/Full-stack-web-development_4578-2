# Git commands 

## Basic config
* update user daetails global:
```bash
$ git config --global user.name <"NAME">
$ git config --global user.email <"EMAIL">
git config --list 
```
* show the git config content with this command:
```bash
cat .gitconfig 
```
* ask git for help
```bash
git --help
git help <"COMMAND">
```

## First git project
```bash
mkdir test  # craete new folder named test

cd test   # change current path to the folder that we created in prev step

ls -a  # show all folder content
./  ../

git init  # Initialized empty Git repository 
Initialized empty Git repository in C:/Users/administrator.NB/test/.git/

ls -a     # show all folder content
./  ../  .git/

touch first.txt   # create a new fike named first.txt

ls -a    # show all folder content
./  ../  .git/  first.txt

echo "test1" > first.txt   # write into first.txt file "test1"

cat first.txt  # show first.txt file content
test1

git status   # command to check untracked / uncommited parts
On branch master
No commits yet
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        first.txt

nothing added to commit but untracked files present (use "git add" to track)

git add . # add to stage all changes that are untracked

git status    # command to check untracked / uncommited parts
On branch master
No commits yet
Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   first.txt

git commit -m "first commit"  # record changes to the repository
[master (root-commit) ba3173a] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 first.txt

git status      # command to check untracked / uncommited parts
On branch master
nothing to commit, working tree clean

```
# Markdown Syntax
## Phrase Emphasis ##

	*italic*   **bold**
	_italic_   __bold__


## Links ##

Inline:

	An [example](http://url.com/ "Title")

Reference-style labels (titles are optional):

	An [example][id]. Then, anywhere
	else in the doc, define the link:
	
	  [id]: http://example.com/  "Title"


## Images ##

Inline (titles are optional):

	![alt text](/path/img.jpg "Title")

Reference-style:

	![alt text][id]

	[id]: /url/to/img.jpg "Title"


## Headers ##

Setext-style:

	Header 1
	========
	
	Header 2
	--------

atx-style (closing #'s are optional):

	# Header 1 #

	## Header 2 ##

	###### Header 6


## Lists ##

Ordered, without paragraphs:

	1.  Foo
	2.  Bar

Unordered, with paragraphs:

	*   A list item.
	
		With multiple paragraphs.

	*   Bar

You can nest them:

	*   Abacus
		* answer
	*   Bubbles
		1.  bunk
		2.  bupkis
			* BELITTLER
		3. burper
	*   Cunning


## Blockquotes ##

	> Email-style angle brackets
	> are used for blockquotes.
	
	> > And, they can be nested.

	> #### Headers in blockquotes
	> 
	> * You can quote a list.
	> * Etc.


## Code Spans ##

	`<code>` spans are delimited
	by backticks.

	You can include literal backticks
	like `` `this` ``.


## Preformatted Code Blocks ##

Indent every line of a code block by at least 4 spaces or 1 tab.

	This is a normal paragraph.

	    This is a preformatted
	    code block.


## Horizontal Rules ##

Three or more dashes or asterisks:

	---
	
	* * *
	
	- - - - 


## Manual Line Breaks ##

End a line with two or more spaces:

	Roses are red,   
	Violets are blue.
 