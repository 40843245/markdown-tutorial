# guide in Obsidian 
## Support
### Markdown 
> [!NOTE]
> Obsidian supports not only some markdown language (such as [CommonMark](https://commonmark.org/), [GFM](https://github.github.com/gfm/)), but also some markup language (such as [LaTex](https://www.latex-project.org/)) However, it does **NOT** support `using Markdown formatting or blank lines inside of HTML tags`.
>
> For more detail about syntax in markdown, see
> + [full guide in markdown (My notes at Github)](https://github.com/40843245/markdown-tutorial/blob/main/full%20guide.md) or
> + [full guide in markdown (My notes at Github) (has TOC)](https://github.com/40843245/markdown-tutorial/blob/main/full%20guide-toc.md)

## Text 
### Heading
Since Obsidian supports some markdown language, the syntax of heading are same as those in markdown language. 

See `MarkdownFile1.md` in `vault2.zip` at Github.

### Paragraph
Since Obsidian supports some markdown language, and all markdown language supports html tag, the syntax of paragraph are same as those in html. 

See `MarkdownFile1.md` in `vault2.zip` at Github.

### Text formatting
Since Obsidian supports some markdown language, the syntax of bold, italic, bold and italic, bold and nested italic in Obsidian are same as those in markdown language. 

In Addition, it supports strikethrough, highlight.

See `MarkdownFile1.md` in `vault2.zip` at Github.

#### Bold text
See `MarkdownFile1.md` in `vault2.zip` at Github.

#### Italic text
See `MarkdownFile1.md` in `vault2.zip` at Github.

#### Bold and Italic text
See `MarkdownFile1.md` in `vault2.zip` at Github.

#### Bold and nested Italic text
See `MarkdownFile1.md` in `vault2.zip` at Github.

#### Strikethrough text
See `MarkdownFile1.md` in `vault2.zip` at Github.

#### Highlight text
See `MarkdownFile1.md` in `vault2.zip` at Github.

## Table
Since Obsidian supports some markdown language, the syntax of table in Obsidian are same as those in markdown language. 

## [Anchor link](https://help.obsidian.md/Linking+notes+and+files/Internal+links#Link+to+a+heading+in+a+note)
One can link to specific headings in notes, also known as anchor links.

See [Anchor link](https://help.obsidian.md/Linking+notes+and+files/Internal+links#Link+to+a+heading+in+a+note)

## Alias
### [Link to a note using an alias](https://help.obsidian.md/Linking+notes+and+files/Aliases#Link+to+a+note+using+an+alias)

The syntax is shown as follows.

```
[[Artificial Intelligence|AI]]
```

The left hand side of `|` indicates a note that will be link.

The right hand side of `|` indicates the text will be displayed.

+ Example 1: (See `alias2.md` in `vault2.zip` at GitHub)

```
# Nickname
## Give it a nickname
[[Artificial Intelligence|AI]]

[[Artificial Intelligence#Intro|AI]]

[[Artificial Intelligence#Intro|AI#Intro]]

[[Artificial Intelligence#See also|AI#Intro]]
```

will be rendered output looks like following screenshot:

![image](https://github.com/user-attachments/assets/36019bab-acd9-47e6-adaf-42833ba6ef9a)

In this example, there are four links.

| item | link name | a note that will be link | displayed text | 
| ----- | -------- | ------------------------ | -------------- |
| `[[Artificial Intelligence\|AI]]` | `Artificial Intelligence` | `Artificial Intelligence.md` | `AI` |
| `[[Artificial Intelligence#Intro\|AI]]` | `Artificial Intelligence#Intro` | `Intro` section in `Artificial Intelligence.md` | `AI` |
| `[[Artificial Intelligence#Intro\|AI#Intro]]` | `Artificial Intelligence#Intro` | `Intro` section in `Artificial Intelligence.md` | `AI#Intro` |
| `[[Artificial Intelligence#See also\|AI#Intro]]` | `Artificial Intelligence#See also` | `See also` section in `Artificial Intelligence.md` | `AI#Intro` |

For full example, see `alias2.md` in `vault2.zip` at GitHub)

## [Backlinks](https://help.obsidian.md/Plugins/Backlinks)

With the Backlinks plugin, you can see all the backlinks for the active note.

A backlink for a note is a link from another note to that note.

> [!NOTE]
> backlinks can be categorized into
> + Linked mentions
> + Unlinked mentions

See the following subsections for more details.

Backlinks provides the following options.
+ Collapse results toggles whether to expand each note to display the mentions in it.
+ Show more context toggles whether to truncate or display the full paragraph that contains the mention.
+ Change sort order determines how to sort the mentions.
+ Show search filter toggles a text field that lets you filter the mentions.

For more information on how to build a search query, refer to [Search](https://help.obsidian.md/Plugins/Search).

+ Example 1: from the official Docs

In the following example, the "Three laws of motion" note contains a link to the "Isaac Newton" note. The corresponding backlink would link from "Isaac Newton" back to "Three laws of motion". 

See the following figure.

![image](https://github.com/user-attachments/assets/c41027ad-46dd-4e94-934c-635b031543fd)

### Linked mentions
Linked mentions are backlinks to the notes that contain an internal link to the active note.

### Unlinked mentions
Unlinked mentions are backlinks to any unlinked occurrence of the name of the active note.






## List
### [Task lists](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Task+lists)

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

#### [With Nested item](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Nesting+lists)

+ Example 1:
  
```
- [ ] Task item 1

	- [ ] Subtask 1

- [ ] Task item 2

	- [ ] Subtask 1
```

will be rendered output looks like following screenshot:

![image](https://github.com/user-attachments/assets/d7b1f8be-c997-431f-9714-ae9a997af2b7)

### [Embed a list](https://help.obsidian.md/Linking+notes+and+files/Embed+files#Embed+a+list+in+a+note)

To embed a list from a different note, first add a block identifier to your list:

```
- list item 1
- list item 2

^my-list-id
```

Then link to the list using the block identifier:

```
![[My note#^my-list-id]]
```

## [Block](https://help.obsidian.md/Linking+notes+and+files/Internal+links#Link+to+a+block+in+a+note)

> [!IMPORTANT]
> It is only availables in Obsidian. NOT in markdown language.

+ Example 1: (See `Block1.md`,`Link to Block1.md`, and `2023-01-01.md` in `vault2.zip` at Github)
  
To create a link that links to `quote-of-the-day` in in `2023-01-01.md`.
1. Define a block named `quote-of-the-day`.
2. Type a block `[[2023-01-01#^quote-of-the-day]]`.

1. Define a block named `quote-of-the-day`:

To add `^quote-of-the-day`  at the end of a block. Type such as 

```
"You do not rise to the level of your goals. You fall to the level of your systems." by James Clear ^quote-of-the-day
### Link a block in a note
```

P.S. can type it in any note.

2. Type a block `[[2023-01-01#^quote-of-the-day]]`:
Now you can link to the block by typing `[[2023-01-01#^quote-of-the-day]]`.


## [Code block](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Code+blocks)
Since Obsidian supports some markdown language, the syntax of code block are same as those in markdown language. 

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

## [Comments](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#Comments)

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

## Callout on Obsidian
### [Supported types](https://help.obsidian.md/Editing+and+formatting/Callouts#Supported+types)

> [!NOTE]
> Unless you Customize callouts, any unsupported type defaults to the `note` type.

> [!NOTE]
> The type identifier is **case-insensitive**.


+ Example 1: (See `Callback0_1.md` in `vault2.zip`)
  
```
> [!TIP]
> Helpful advice for doing things better or more easily.

> [!hint]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/f1f4bc4b-5ddc-4053-a989-cb7b2039e5a3)

+ Example 2: (See `Callback0_2.md` in `vault2.zip`)
  
```
> [!abstract] 
> Lorem ipsum dolor sit amet

> [!summary] 
> Lorem ipsum dolor sit amet

> [!tldr] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/9a967840-e065-4366-ba6f-d5f710b19385)

+ Example 3: (See `Callback0_3.md` in `vault2.zip`)
  
```
> [!todo] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/0b654cab-e599-4e14-8efe-48892a866100)

+ Example 4: (See `Callback0_4.md` in `vault2.zip`)
  
```
> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
>  Advises about risks or negative outcomes of certain actions.

> [!attention]
>  Advises about risks or negative outcomes of certain actions.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/1607448e-fb60-43bc-9f8f-69cf6ed8ee30)

+ Example 5: (See `Callback0_5.md` in `vault2.zip`)
  
```
> [!info] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/e100309a-7e92-4446-9510-2b4eaef313d4)

+ Example 6: (See `Callback0_6.md` in `vault2.zip`)
  
```
> [!success] 
> Lorem ipsum dolor sit amet

> [!check] 
> Lorem ipsum dolor sit amet

> [!done] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/5ccaf2a5-31ad-40b5-a231-42deb4fc0784)

+ Example 7: (See `Callback0_7.md` in `vault2.zip`)
  
```
> [!question] 
> Lorem ipsum dolor sit amet

> [!help] 
> Lorem ipsum dolor sit amet

> [!faq] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/a186a904-6b3e-439c-92e8-0305de0275c3)

+ Example 8: (See `Callback0_8.md` in `vault2.zip`)
  
```
> [!note] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/044362f5-f550-44aa-8eec-ad173b9db1f4)

+ Example 9: (See `Callback0_9.md` in `vault2.zip`)
  
```
> [!failure] 
> Lorem ipsum dolor sit amet

> [!fail] 
> Lorem ipsum dolor sit amet

> [!missing] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/5ad52ff4-f9d3-4503-992e-481e8f5f7eed)

+ Example 10: (See `Callback0_10.md` in `vault2.zip`)
  
```
> [!danger] 
> Lorem ipsum dolor sit amet

> [!error] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/0581fd83-60b5-4dc3-89c6-ab4c2511a444)

+ Example 11: (See `Callback0_11.md` in `vault2.zip`)
  
```
> [!bug] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/8d2c8a8d-06f6-4713-aee7-984d752f8c79)

+ Example 12: (See `Callback0_12.md` in `vault2.zip`)
  
```
> [!example] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/dd1790c8-cde2-48ac-84c5-4216dc67cb06)

+ Example 13: (See `Callback0_13.md` in `vault2.zip`)
  
```
> [!quote] 
> Lorem ipsum dolor sit amet

> [!cite] 
> Lorem ipsum dolor sit amet
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/0a330b9a-526f-4b6d-bfe5-86a24a266282)


### Nested item in callout

+ Example 1: (See `Callback1.md` in `vault2.zip`)

```
> [!info]
>  Here's a callout block.
> It supports **Markdown**, [[Internal link|Wikilinks]], and [[Embed files|embeds]]!
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/0d1c5ebf-fee1-4cc1-aee7-c1213d9e1cef)

+ Example 3:

```
> [!faq]
> - Are callouts foldable? 
> - Yes! In a foldable callout, the contents are hidden when the callout is collapsed.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/90c14029-7208-4a9a-aa86-dca446f7122f)

### Change the title of callout
By default, the title of the callout is its type identifier in title case. 

One can change it by adding text after the type identifier. (See Example 1)

One can even omit the body to create title-only callouts. (See Example 2)

+ Example 1: (See `Callback2.md` in `vault2.zip`)

```
> [!tip] Callouts can have custom titles 
> Like this one.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/0ffba3d8-37fe-4e11-af19-c2c4e55234c7)


+ Example 2: (See `Callback3.md` in `vault2.zip`)

```
> [!tip] Title-only callout 
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/70cea76f-1064-45b1-a6bc-ab88c688145a)

### Foldable callout

To add a foldable callout, add consecutive `-` after `]`. 

> [!NOTE]
> Don't leave any characters between `]` and `-`. Otherwise, the callout will NOT be foldable.

+ Example 1: (See `Callback4.md` in `vault2.zip`)

```
> [!faq]- Are callouts foldable? 
> - Yes! In a foldable callout, the contents are hidden when the callout is collapsed.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/8cc422e4-de22-412a-9a0a-e92b67ab7dfa)

+ Example 2: (See `Callback5.md` in `vault2.zip`)

```
> [!faq]-
> - Yes! In a foldable callout, the contents are hidden when the callout is collapsed.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/d4c9d5b6-d414-45a4-a67e-ea80ce5cb340)

#### Nested foldable callout

+ Example 1: (See `Callback6.md` in `vault2.zip`)

```
> [!question] Can callouts be nested? 
> > [!todo] Yes!, they can. 
> > > [!example] You can even use multiple layers of nesting.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/a2e2d8b2-3053-4bf1-88c8-63a65b531cff)

### [Customized callout](https://help.obsidian.md/Editing+and+formatting/Callouts#Customize+callouts)

+ Example 1: (See `Callback7.md` in `vault2.zip`)

1. Create a css file (here I named it as `customized_callout_css1.css`) under `.../.obsidian/snippets`.

2. Add the following in the css file.

```
.callout[data-callout="custom-question-type"] {
    --callout-color: 255, 128, 128;
    --callout-icon: lucide-alert-circle;
}
```

3. Then one uses a callout with identifier `custom-question-type`. (i.e. `[!custom-question-type]` ). The css style will be applied.

```
> [!custom-question-type]
> This is a callout.
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/b34b7be0-5ea3-4b2e-a745-df55f60df0a2)

## File
### Internal file

To embed a file.

Type `!` followed by `[`, then your file name , finally closed by `]`.

```
![RFC 2181 (full documentation,original).pdf]
```

For more details, see following example.

#### PDF

As same as embeding a file in Obsidian.
  
To embed a pdf file named `RFC 2181 (full documentation,original).pdf`. Type

```
![[RFC 2181 (full documentation,original).pdf]]
```

One can also open a specific page in the PDF, by adding `#page=N` to the link destination, where N is the number of the page. 

To open `RFC 2181 (full documentation,original).pdf` at third page. Type 

```
![[RFC 2181 (full documentation,original).pdf#page=3]]
```

One can also specify the height in pixels for the embedded PDF viewer, by adding `#height=[number]` to the link. 

To open `RFC 2181 (full documentation,original).pdf` with `height` `400`. Type

```
![[RFC 2181 (full documentation,original).pdf#height=400]]
```

+ Example 1: Import a PDF file. (See `Import PDF.md` in `vault2.zip`)

Here is the file structure in file explorer.

![image](https://github.com/user-attachments/assets/77f5c77a-ac3a-4c4f-bc73-f245681ab41e)

1. Create a note named `Import PDF` and type `Import PDF` as title. 

2. Type these content in following code block.

```
![[RFC 2181 (full documentation,original).pdf]]
```

Shown as following figure.

![image](https://github.com/user-attachments/assets/2d7a7981-e435-4e2a-ab22-81c2450e80e6)

Then you will see the content of `RFC 2181 (full documentation,original).pdf` in Obsidian note.

Shown as following figure.

![image](https://github.com/user-attachments/assets/f8c981ef-c66e-4eb3-9da3-4af861a95c17)

#### Image
##### [Images that specifies the width or height etc](https://stackoverflow.com/questions/14675913/changing-image-size-in-markdown)

Take `Import Figure.md` in `vault1.zip` at Github as example. To illustrate the example, do the following step.

1. Download [`vault1.zip` at Github](https://github.com/40843245/tool/blob/main/markdown/extensions%20tool/Obsidian/attachment/vault1.zip)
2. Unzip the file.
3. Open `Import Figure.md`.
4. View it with source mode.
5. View it with Editor View mode.
6. View it with Reading View mode.

After you view the file with many modes (such as source mode, Editor View mode, Reading View mode, you will understand how it works.

## Video
### YT Video
#### [Embed a YouTube video](https://help.obsidian.md/Editing+and+formatting/Embed+web+pages#Embed+a+YouTube+video)

To embed a YouTube video, use the same Markdown syntax as external images:

+ Example 1: (See `Embed YT Video.md` in `vault2.zip` at Github)
  
```
![](https://www.youtube.com/watch?v=NnTvZWp5Q7o)
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/0c68e8a0-797f-40c3-8e2c-f1508ee48085)

## Social media
### Tweet
#### [Embed a tweet](https://help.obsidian.md/Editing+and+formatting/Embed+web+pages#Embed+a+tweet)

To embed a tweet, use the same Markdown syntax as external images:

+ Example 1: (See `Embed YT Video.md` in `vault2.zip` at Github)
  
```
![](https://twitter.com/obsdmd/status/1580548874246443010)
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/b03bbc32-ac98-4e0d-a45f-3d2108f9e56c)

## Style
### Change style

To use customized style.
1. Create a customized style.
2. Apply the customized style.

For example, see `vault2.zip` file at Github.

About syntax on css in Obsidian, see [css variable in Obsidian](https://docs.obsidian.md/Reference/CSS+variables/CSS+variables)

### Create a customized style
1. Create a css file under `.../.obsidian/snippets` folder.
    
### Apply a customized style
1. Select `settings`->`Appearance`.
2. Under `CSS snippets`, click `Reload` button to refresh it.
3. Under `CSS snippets`, toggle on the css snippet that you want to apply.

### Unapply a customized style
1. Select `settings`->`Appearance`.
2. Under `CSS snippets`, toggle off the css snippet that you want to apply.

## Property

> [!NOTE]
> Properties allow you to organize information about a note.
> Properties contain structured data such as text, links, dates, checkboxes, and numbers.
> Properties can also be used in combination with Community plugins that can do useful things with your structured data.

### [Add properties to a note](https://help.obsidian.md/Editing+and+formatting/Properties#Add+properties+to+a+note)
There are several ways to add a property to a note.
+ Use the `Add file property` command.
+ Use the `Cmd/Ctrl`+`;` hotkey.
+ Choose `Add file property1 from the `More actions menu` (brought up by the three dots icon or by right-clicking the tab).
+ Type `---` at the very beginning of a file.

### [Property types](https://help.obsidian.md/Editing+and+formatting/Properties#Property+types)

Obsidian supports the following property types.
+ Text
+ List
+ Number
+ Checkbox
+ Date
+ Date & time

> [!IMPORTANT]
> Once a property type is assigned to a property, all properties with that name are assumed to have the same property type.

### Search property
See next subsection `Search property` in `Search plugins` section.

## [Search plugins](https://help.obsidian.md/Plugins/Search)
### [Search properties](https://help.obsidian.md/Plugins/Search#Search+properties)

Use brackets around a property name `[yourProperty]` to return files with that property `yourProperty`.

Use brackets and a colon `[yourProperty:yourValue]` to return files with that property `yourProperty` and value `yourValue`.

+ Example 1: (See `vault2.zip` at Github)

Take `vault2.zip` at Github as example.

In search box, type

```
[tag:YT] 
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/2aaa2978-dbaa-4b00-9dcf-5aa54d6e4545)

### [Search operators](https://help.obsidian.md/Plugins/Search#Search+operators)
Available search operators at [Search operators](https://help.obsidian.md/Plugins/Search#Search+operators).

## Search results
### [Copy search results](https://help.obsidian.md/Plugins/Search#Copy+search+results)
1. Enter a search term.
2. Under the search field, select the three dots icon next to the number of results.
3. Select `Copy search results`.
4. One will see the following popup for instance.

![image](https://github.com/user-attachments/assets/5d29dfb2-c177-499e-b280-749a65bb84eb)

5. Make up the settings of popup.
6. Click `Copy results` in the popup.

For demo, see my YT video [Copy search results in Obsidian.](https://www.youtube.com/watch?v=wWxgTl_nUBk).

### [Sort search results](https://help.obsidian.md/Plugins/Search#Change+result+sort+order)
1. Enter a search term.
2. Under the search field, click on the dropdown on the right.
3. Select the sort order you want. Default is "File name (A to Z)".

For demo, see my YT video [Sort search results in Obsidian](https://www.youtube.com/watch?v=5DcwCz0iYjE).

### get explanation of search query
1. Enter a search term.
2. Click the filter icon. Shown as follows

![image](https://github.com/user-attachments/assets/2cc2dbe6-6f03-49e8-be6b-799079657aef) 

3. Toggle on `Explain search terms`.

For demo, see my YT video [get explanation of search query in Obsidian](https://www.youtube.com/watch?v=o5Tr9HJu7kY).

### [search results case sensitively](https://help.obsidian.md/Plugins/Search#Change+case+sensitivity)
1. Click match case icon 'Aa'. Shown as follows.

![image](https://github.com/user-attachments/assets/55acfa63-8437-4a39-bed6-c2d23b31844f)

For demo, see my YT video [search results case sensitively in Obsidian](https://www.youtube.com/watch?v=qfdqTL7hqNA).
   
### [Embed search results in a note](https://help.obsidian.md/Plugins/Search#Embed+search+results+in+a+note)

To embed search results in a note, add a query code block:

+ Example 1: (See `Embed search results in a note.md` in `vault2.zip` at Github)
  
```
\`\`\`query
embed OR search
\`\`\`
```

will render output looks like as following screenshot:

![image](https://github.com/user-attachments/assets/68eefe6a-ec7d-49ee-84f3-c89369a0f5f8)

> [!NOTE]
> Obsidian Publish doesn't support embedded search results.
> To see a live rendered example, use the code block above within your vault.
