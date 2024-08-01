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


