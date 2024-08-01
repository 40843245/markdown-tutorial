# syntax in Obsidian 
## Support
### Markdown 
> [!NOTE]
> Obsidian supports not only some markdown language (such as [CommonMark](https://commonmark.org/), [GFM](https://github.github.com/gfm/)), but also some markup language (such as [LaTex](https://www.latex-project.org/)) However, it does **NOT** support `using Markdown formatting or blank lines inside of HTML tags`.
>
> For more detail about syntax in markdown, see
> + [full guide in markdown (My notes at Github)](https://github.com/40843245/markdown-tutorial/blob/main/full%20guide.md) or
> + [full guide in markdown (My notes at Github) (has TOC)](https://github.com/40843245/markdown-tutorial/blob/main/full%20guide-toc.md)



## [Task lists](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Task+lists)

> [!IMPORTANT]
> It is only available in Obsidian note.

To create a task list, start each list item with a hyphen and space followed by [ ].

+ Example 1:
  
```
- [x] This is a completed task.

- [ ] This is an incomplete task.
```

will be rendered output looks like following screenshot:

![image](https://github.com/user-attachments/assets/0b7f2d2e-89e8-453d-8772-f325c7d4ec5d)

> [!TIP]
> You can use any character inside the brackets to mark it as complete.

+ Example 2:

```
- [x] Milk
- [?] Eggs
- [-] Eggs
```

will be rendered output looks like following screenshot:

![image](https://github.com/user-attachments/assets/4e564e52-f3ef-4634-9493-c0a7c907e4d1)

### [Nested item](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Nesting+lists)

+ Example 1:
  
```
- [ ] Task item 1

	- [ ] Subtask 1

- [ ] Task item 2

	- [ ] Subtask 1
```

will be rendered output looks like following screenshot:

![image](https://github.com/user-attachments/assets/d7b1f8be-c997-431f-9714-ae9a997af2b7)

## Code block
### [Syntax highlighting](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Code+blocks)

See [Syntax highlighting](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Code+blocks)

## Footnotes

Not only Obsidian support non-inline footnotes (as Obsidian support markdown language), but also it supports inline footnotes.

### Non-inline footnotes

See my notes about markdown (in Markdown section).

### Inline footnotes

> [!NOTE]
> Inline footnotes only work in reading view, not in Live Preview.

+ Example 1:
  
```
^[This is an inline footnote.]
```

will be rendered output looks like following screenshot:
	
![image](https://github.com/user-attachments/assets/4c7c304e-42a9-46d4-9ef0-aee0286ea577)

## [Comments]

Obsidian support not only non-inline comments but also inline comments.

### Inline comments

```
This is an %%inline%% comment.
```

will be rendered output looks like following screenshot in Reading View mode: 

![image](https://github.com/user-attachments/assets/4fbeb9f5-f2c6-4055-b57f-3e8f436dab82)

### Non-inline comments

```
This is a block comment.
%%
Block comments can span multiple lines.
%%
```

will be rendered output looks like following screenshot in Reading View mode: 

![image](https://github.com/user-attachments/assets/42d28416-1393-4f7a-90b0-125ae23c5b2e)

## [Internal Link](https://help.obsidian.md/Linking+notes+and+files/Embed+files#Embed+a+note+in+another+note)

one can embed a note through `internal link`

+ Example 1:

1. Create a note named `Internal links` (or open existing one named `Internal links`), 

type `Internal links` as title.

Then type these contents in code block in the note.

```
#^b15695
This is a section.
```

shown as follows.

![image](https://github.com/user-attachments/assets/a7919353-7b7b-464e-83d4-48aecbda55f5)

2. Create a note named `Other notes` (or open existing one named `Other notes`),

type `Other notes` as title.   

Then type these contents in code block in the note.

```
![[Internal links]]
```

will be rendered output looks like following screenshot in Reading View mode: 

![image](https://github.com/user-attachments/assets/ce022407-8175-48fc-b203-e61557c30a49)

## Image
### [Images that specifies the width or height etc](https://stackoverflow.com/questions/14675913/changing-image-size-in-markdown)

Let's look at images the size is **NOT** changed and its syntax first, then, look at images that the width or height is specified, and its syntax, through following exmaple.

> [!IMPORTANT]
> > They have same effect at Github. However, they may have different effect in different platforms.


+ Example 1: The size is **NOT** changed.

```
![CNAME_ex1](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)
```

will render output looks like this:

![CNAME_ex1](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)

+ Example 2:

```
![CNAME_ex1|20x100](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)
```

will render output looks like this:

![CNAME_ex1|20x100](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)

+ Example 3: 

```
![<img alt='CNAME_ex1' src='https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg' width='20'/>](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)
```

will render output looks like this:

![<img alt='CNAME_ex1' src='https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg' width='20'/>](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)

+ Example 4: 

```
![<img alt='CNAME_ex1' width='20'/>](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)
```

will render output looks like this:

![<img alt='CNAME_ex1' width='20'/>](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)

+ Example 5:

```
![CNAME_ex1\|20x100](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)
```

will render output looks like this:

![CNAME_ex1\|20x100](https://github.com/40843245/computer-science/blob/main/attachment/paradigm/CNAME_ex1.jpg)

## Alert on Obsidian

+ Example 1:
  
```
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/bc940a36-3b60-4312-8bfd-9d0dd15f1aa9)

## File
### Internal file

+ Example 1: Import a file.

Here is the file structure in file explorer.

![image](https://github.com/user-attachments/assets/77f5c77a-ac3a-4c4f-bc73-f245681ab41e)

1. Create a note named `Import PDF` and type `Import PDF` as title. 

Shown as following figure.

![image](https://github.com/user-attachments/assets/2d7a7981-e435-4e2a-ab22-81c2450e80e6)

Then you will see the content of `RFC 2181 (full documentation,original).pdf` in Obsidian note.

Shown as following figure.

![image](https://github.com/user-attachments/assets/f8c981ef-c66e-4eb3-9da3-4af861a95c17)


will render output looks like as following screenshot:

