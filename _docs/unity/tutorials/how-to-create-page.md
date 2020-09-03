---
title: How To Create Page
layout: docs
category: Unity 7
---
This is a guide how to create page for github documentation site using Markdown syntax. If you know Markdown syntax, start from [Markdown file structure and page structure](../how-to-create-page/#markdown-file-structure-and-page-structure).  

# Markdown Syntax 

## Headings 

To create a heading, add number signs (#) in front of a word or phrase:   
```
# Heading Level 1  
## Heading level 2  
### Heading level 3 
#### Heading level 4   
```
Heading Level 1 is the biggest. 
Don't forget type a space between `#` and `Heading`. 

## Paragraphs 

To create paragraphs, use a blank line between text lines. Don't put tabs or spaces in front of your paragraphs.  
```
This is the first paragraph of text.

This is the second paragraph of text.
```

## Line breaks 

To create a line break, end a line with two or more spaces, and then press `Enter`.  
Next text will be on the next line. 
```
This is the first line of paragraph.  
This is the second line of paragraph. 
```

## Lists 

To organize items in unordered list, type: 
```
- First item  
- Second item  
- Third item 
``` 
It will look on page:  
- First item
- Second item
- Third item  

To organize items in ordered list, type:
``` 
1. First item
2. Second item
3. Third item 
```

It will look on page: 
1. First item
2. Second item
3. Third item 

## Links 

To create a link, type: 
```
[Title of link](url)
```
It will look on page:  
[Title of link](url) 

## Images 

To insert an image, type: 
```
![Title of image](url)
``` 

To align left edge of the image with text in list, use `tab` before `![Title of image](url)` 

## Code and code blocks 

To denote a word or phrase as code, enclose it in backticks (`):

```
`code word` 
```

It will look on page: 

`code word` 

To create code block, use three backticks (```) on the lines before and after the code block: 

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

Many Markdown processors support syntax highlighting for fenced code blocks. 
To highlight code, add `json` just after three backticks before the code block: 

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

## Tables 

To create a table, type: 
```
| Column 1     | Column 2     |
| ------------ | ------------ |
| cell content | cell content |
| cell content | cell content |
```
It will look on page: 

| Column 1     | Column 2     |
| ------------ | ------------ |
| cell content | cell content |
| cell content | cell content | 

To align columns to the left or right edge, add `:` sign: 
```
| Column 1             | Column 2          |
| :------------------- | ----------------: |
| left                 | right             |
| alignment            | alignment         |
```
It will look on page: 

| Column 1             | Column 2          |
| :------------------- | ----------------: |
| left                 | right             |
| alignment            | alignment         |

You can add links, code (words or phrases in backticks (`) only, not code blocks), and emphasis.
You can’t add headings, blockquotes, lists, horizontal rules, images, or HTML tags.  
Use [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables) to create tables. 

## Emphasis 

To **bold** text, add two asterisks before and after word or phrase: `**bold**`

## Blockquotes 

To create a blockquote, add a > in front of a paragraph: 

```
> This is a citation from another document  
```
It will look on page: 

> This is a citation from another document  


For additional information about Markdown syntax see:  
- [https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/)  
- [https://www.markdownguide.org/extended-syntax/](https://www.markdownguide.org/extended-syntax/)

# Markdown file structure and page structure 

## Metadata in the beginning of .md file 

```
---
title: New Page Template
layout: docs
category: Unity 7
---
```
This information is not visible on site page, but required to properly embed page in the site.
Sidebar.yml file should contain the same `title` value. 

## Title of page 
 
Don't type title of page in markdown file. It will appear on page automatically from metadata above.   

## Table of contents 

Table of contents is created automatically from headers on page. It is important to headline chapters and subitems accordingly to their hierarchy.  

## Content of page  

### Text 

Use `# Heading Level 1` with all capital letters to write titles of chapters. 

Use `## Heading level 2`, `### Heading level 3` and `#### Heading level 4` with only first capital letter to write subchapters.  

Use backticks (`) to write: 
- commands and messages in Command Prompt: `cd C:\DockerUnity\`, `Login Succeeded` 
- names and paths to directories and files: `C:/DockerUnity` 
- paths to sections: `Resources > File sharing` 
- buttons: `Apply` button  

Bold text is automatically used in tables for column titles. 
Also use bold text: 
- to emphase important notes (just word **Note:** should be bold, not text after it) 
- to title parts of text like **Problem** and **Solution** in Troubleshooting chapter  

Use blockquotes to write quotes from an external sources. 

Use plain text for the rest of content.  

### Lists 

Unordered lists are preferrable. Use ordered lists if only it is necessary to count items. 

### Code blocks 

Use simple or highlighted code blocks. 

### Images and screenshots requirements 

- Preferrable image format is .png 
- Screenshots to illustrate process steps should have the same size 
- Crop screenshots accurately 
- For highlighting use red frames, red color is R220 G56 B64 (#dc3840):  
	![highlight](../images/how-to-create-page/image10.png) 
- Use `:` after the text before image if image illustrates this text 

Images should be placed to `../images/name-of-your-md-file/` folder. 

### Tables 

The simpler the better. Big tables might be rendered unpredictable. 

### Confidential information 

Remove all confidential information from your content and images (passwords etc).

## Next step recommendations (optional) 

You can type at the end of the page a source for the next step:  

`&rarr; [Next step: Next Page Title](path/next-page-title/)`  

It will look on page: 

&rarr; [Next step: Next Page Title](./next-page-title/)



