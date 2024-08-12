# markdown metedata format
## YAML Front Matter
+ Example 1:

```
---
layout: post
title: Blogging Like a Hacker
---
```

## MultiMarkdown Metadata
+ Example 1:

```
Title:    A Sample MultiMarkdown Document  
Author:   Fletcher T. Penney  
Date:     February 9, 2011  
Comment:  This is a comment intended to demonstrate  
          metadata that spans multiple lines, yet  
          is treated as a single value.  
CSS:      http://example.com/standard.css
```

## Pandoc Title Block
+ Example 1:

```
% title
% author(s) (separated by semicolons)
% date
```

## A workaround use standard syntax and compatible with all other viewers

+ Example 1:

```
  [_metadata_:author]:- "daveying"
  [_metadata_:tags]:- "markdown metadata"
```

## Ref
[Markdown metadata format](https://stackoverflow.com/questions/44215896/markdown-metadata-format)
