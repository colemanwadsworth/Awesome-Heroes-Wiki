# Wiki Guide

One of the most important things to understand when making an effective wiki is folder nesting.  You want to go from general to specific in a logical way so that it is easier to deal with all the data that will start to build up.  Otherwise it will become hard to process the data and not as useful to have it.

### To Create A New File
These will create files inside the root directory. That means the main folder all your files are in.
```
[[Name Of Link|name-of-file]]

OR

[[Name Of Link|filename]]
```

These will create files inside another folder:
```
[[Name Of Link|foldername/name-of-file]]

The file structure now looks like:

Wiki (root directory)
|  
+__Main Wiki File
|
+__foldername
        |
        +__name-of-file

OR

[[Name Of Link|foldername/filename]]

Wiki (root directory)
|  
+__Main Wiki File
|
+__foldername
        |
        +__filename

```
Getting back to effectively organizing your files.  Here is an example of  intelligently nested files and the links that will create those files:
```
[[Animals|animals/types-of-animals]]

# Now lets imagine we go to the page animals/types-of-animals on this page we might create something like:

[[Mammals|animals/mammals/content]]
[[Reptiles|animals/reptiles/content]]
[[Birds|animals/birds/content]]

# This is what the file structure for the wiki would now look like:

Wiki (root directory)
|
+__animals(subdirectory)
      |
      |_mammals(sub/subdirectory)
      |         |
      |         +_content(file that can act as table of contents for mammals)
      |
      |_reptiles(sub/subdirectory)
      |         |
      |         +_content(file that can act as table of contents for mammals)
      |
      |_birds(sub/subdirectory)
                |
                +_content(file that can act as table of contents for mammals)

```

When you first create a new file using the ```[[Link Name|filename]]``` notation it will start off looking RED. When you click on the link it will turn create the file for you automatically and when you save it that link will then turn BLUE.

When you click on a red link and it brings you to a new blank page you are going to want to create a header for the page.  That way the top of the page will display what that wiki page is about.  The way to create headers in markdown is to use the hashtag symbol ```#```.

Depending on how many hashtags you use the size of the header will be bigger or smaller. However, the first instance of a single header will automatically create the header for a page.

For example:
```
# Mammals
```
That will make the page display Mammals at the top.

Headers are also useful for separating content on a given page.  In HTML there are different sized headers so you can organize your content more efficiently. Here is how you change the size of the headers:
```
# Biggest header
## Little smaller
### Little smaller
#### little smaller
##### little smaller
###### smallest
```
# Biggest header
## Little smaller
### Little smaller
#### little smaller
##### little smaller
###### smallest

Above is an example of the sizes written in markdown so you can see.

That's really all you need to know in create new pages, folders, and organized content.  There are however a few more things to learn in markdown that are useful to learn in order to organize your content even more efficiently. [This is a link to the official markdown page that you can browse to find answers on how to do certain things.](http://daringfireball.net/projects/markdown/)

### Creating Links To External Websites

To create a link like the one above to the markdown official docs you can do the following:

```
[Google](http://www.google.com)
```
In live form:
[Google](http://www.google.com)

### Making Words On New Lines
One of the interesting features of markdown (what you're using to write your wiki) is how it creates new lines for you.  Instead of having to create complicated HTML all you need to do is add two spaces at the end of a line and it will automatically start new text on a new line.

You can also just hit enter a few times and that should work as well.

Heres an example to explain:
```

[google](http://www.google.com)
[facebook](http://www.facebook.com)

those two links would look like this:
googlefacebook

To fix that make sure to add the two spaces
[google](http://www.google.com)__
[facebook](http://www.facebook.com)__

(Since I can't write spaces pretend those two underscores are spaces) Now the links will look like this:

google
facebook
```

### Making Lists With Markdown
Making lists is pretty inevitable when it comes to organizing information. Markdown makes it extremely easy.  Here is how to make an unordered list:
```
* list item 1  
* list item 2  
* list item 3  
* list item 4  
```
That would look like:  
* list item 1  
* list item 2  
* list item 3  
* list item 4  

To make an ordered list you would do this:
```
1. list item 1  
2. list item 1  
3. list item 1  
4. list item 1  
```
That would look like:  
1. list item 1  
2. list item 1  
3. list item 1  
4. list item 1  

Notice how you don't actually need to provide the correct numbers.

### Separating Sections Of Content
```
---
```

---


### Italics & Bold
```
**Bold**
__Italics__
```
**Bold**  
_Italics_

### Starting it up:
```
cd desktop/awesome_wiki  
gollum
```