# Mastering Markdown on GitHub
Markdown is a lightweight and easy-to-use syntax for styling all forms of writing on the GitHub platform.

## What is Markdown?
**markdown** is away to style text on the web. you control the display of the document;formating words as **bold** or *italic* adding images 
![image](https://media.sproutsocial.com/uploads/2017/02/10x-featured-social-media-image-size.png)
and creating lists 
1. first
3. second 
5. third 
 
 **are** just a few of the thing we can do with markdown.
  
  ![image](https://d33v4339jhl8k0.cloudfront.net/docs/assets/545804d8e4b09c5ca72525ce/images/5bfffa1304286304a71cca67/file-HkUrvqZYBI.png)

  ## headers

  ![image](https://www.qoncious.com/sites/default/files/q_a_images/ghost_markdown_heading.PNG)

  Lists

Unordered and Ordered

![image](https://i.stack.imgur.com/JSbJ3.png)

Images

![image](https://i2.wp.com/corelab.blog/wp-content/uploads/2020/04/Schermata-2020-04-15-alle-16.53.59.png?resize=383%2C172&ssl=1)


links 

![image](https://1.bp.blogspot.com/-N4e_emEN-nI/W8POCzp8UlI/AAAAAAAAxrI/OvLag5aWsaMV2jfFEaP3o5lRv_xNGgPIQCLcBGAs/s1600/Markdown-sample-codes.png)

Blockquotes

![image](https://i.redd.it/dhv15fftnd131.jpg)

Inline code

I think you should use an
`<addr>` element here instead.

   
# GitHub pages

Create a repository 

![image](http://www.malgreve.net/wp-content/uploads/2014/02/GitHub-Create-New-Repository.png)

Clone the repository

`git clone https://github.com/username/username.github.io` (the repo link)

`cd username.github.io`(cd to the repo)



Push it:

Add, commit, and push your changes:

` git add .`

`git commit -m "Initial commit"`

`git push -u origin main`

# GitHub Markdown Syntax

**Basic writing and formatting syntax**

## Headings:

`# The largest heading`

`## The second largest heading`

`###### The smallest heading`

**bold**

`**This is bold text**`

*Italic*

`*This text is italicized*`

~~Strikethrough~~

`~~This was mistaken text~~`

**This text is _extremely_ important**

`**This text is _extremely_ important**`

***All bold and italic***

`***All this text is important***`

Quoting text
You can quote text with a `>`

In the words of Abraham Lincoln:

> Pardon my French

Quoting code:

Use `git status` to list all new or modified files that haven't yet been committed.

Links:
you can create an inline link by wrapping link text in brackets [ ], and then wrapping the URL in parentheses ( )

Section links:

[Headings](##Heading)



Relative links:

[readme file](README.md)

Lists:

unorder :

`* first`

`* second`

`* third`

* first
* second
* third

to order your list, precede each line with a number
`1. first`
`5. second`
`8.third`
1. first
5. second
8. third

Nested Lists:
```
1. First list item
   - First nested list item
     - Second nested list item 
   ``` 

***
* first
  * second
    * third




     To create a nested list using the web editor on GitHub or a text editor that uses a monospaced font, like Atom, you can align your list visually. Type space characters in front of your nested list item, until the list marker character (- or *) lies directly below the first character of the text in the item above it.




     
     
     #### Task lists:

To create a task list, preface list items with a regular space character followed by [ ]. To mark a task as complete, use [x].

- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request

Mentioning people and teams:
You can mention a person or team on GitHub by typing @ plus their username or team name. 
***


Paragraphs:
You can create a new paragraph by leaving a blank line between lines of text.

Ignoring Markdown formatting
You can tell GitHub to ignore (or escape) Markdown formatting by using \ before the Markdown character.

`Let's rename \*our-new-project\* to \*our-old-project\*.`






