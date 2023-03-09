# Markdown Cheat Sheet 📝
A collection of the most useful and popular syntax for producing articles in Markdown.

## 📌 Create Headers 

# 1. H1 - `#` 

## 2. H2 - `##` 

### 3. H3 - `###` 

#### 4. H4 - `####` 

##### 5. H5 - `#####` 

###### 6. H6 - `######`

<br>

## 📌 Add Typographical Emphasis
> The space between `* *` is where your text is placed.

### 1. Bold text - `** **` OR `__ __`
- This is **bold**, also __these__.

### 2. Italic text - `* *` OR `_ _`
- Italic *text*, also _these_.

### 3.  Strike through - `~~ ~~`
- This was ~~mistaken text~~.

### 4. Bold and nested italic - `** _ _ **`
- **This text is _exrtemely_ important.**

### 5. All bold and italic - `*** ***`
- ***All this text is important***.

### 6. Superscript - `<sup> </sup>` OR `^ ^`
- These text is <sup>superscripted.</sup>

### 7. Subscript - `<sub> </sub>` OR `~ ~`
- These text is <sub>subscripted.</sub>

<br>

## 📌 Quoting Text

Leave an empty space after this `>` and start typing your text to make a quote.
```markdown
Text that is not a quote

> Text that is a quote
```
Text that is not a quote
> Text that is a quote

<br>

## 📌 Quoting Code

### 1. Single backticks  - ``` ` ` ```
  - Call out code or a command *within a sentence* with `single backticks`.

### 2. Triple backticks
````markdown
``` 

```
````
-  Format code or text into its own distinct block.
````git
Some basic Git commands are:
```
$ git status
$ git add
$ git commit
```
````
###### For more information, see "[Creating and highlighting code blocks](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks)."

<br>

## 📌 Add Code and Syntax
- Just type the three backticks followed by the programming language and then enter to start writing your code. End the code block with three backticks.
````
```javascript
console.log('example log')
```
````
Output:
```javascript
console.log('example log')
```

<br>

## 📌 Make Lists

### 1. Unordered list - `-`, `*`, or `+`.
```markdown
- George Washington
* John Adams
+ Thomas Jefferson
```
![Unordered list](https://docs.github.com/assets/cb-3302/mw-1000/images/help/writing/unordered-list-rendered.webp)

### 2. Ordered list - *precede each line with a number.*
```markdown
1. James Madison
2. James Monroe
3. John Quincy Adams
```
![Ordered list](https://docs.github.com/assets/cb-3403/mw-1000/images/help/writing/ordered-list-rendered.webp)

### 3. Nested lists - *indenting one or more list items below another item.* 
```markdown
1. First list item
   - First nested list item
     - Second nested list item
```
![Nested List](https://docs.github.com/assets/cb-5185/mw-1000/images/help/writing/nested-list-alignment.webp)

1. First list item
   - First nested list item
     - Second nested list item

Learn more about [nested lists.](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#further-reading:~:text=John%20Quincy%20Adams-,Nested%20Lists,-You%20can%20create)

### 4. Task lists -  preface list items with a hyphen `-` and space ``` ` ` ``` followed by `[ ]`. To mark a task as complete, use `[x]`.
```markdown
- [x] #739
- [ ] [Keep issue state and checkboxes in sync](https://github.com/octo-org/octo-repo/issues/740) #740
- [ ] Add delight to the experience when all tasks are complete :tada:
```
- [x] #739
- [ ] [Keep issue state and checkboxes in sync](https://github.com/octo-org/octo-repo/issues/740) #740
- [ ] Add delight to the experience when all tasks are complete 🎉

Learn more about [task lists.](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#further-reading:~:text=Markdown%20Spec.-,Task%20lists,-To%20create%20a)

<br>

## 📌 Create Links

### 1.  Inline link - `[ ]( )`
- Create by wrapping link text in brackets `[text]`. and then wrapping the URL in parentheses `(URL)`.
  - You can also use the keyboard shortcut `Command`+`K`.
  - You can also create a Markdown hyperlink by highlighting the text and using the keyboard shortcut `Command`+`V`.
```markdown
This site was built using [GitHub Pages](https://pages.github.com/).
```
This site was built using [GitHub Pages](https://pages.github.com/).

### 2. Section link ✒
- link directly to a section in a rendered file by hovering over the section heading to expose the link:

### 3. Relative links 📂
- Define relative links and image paths in your rendered files to help readers navigate to other files in your repository.
- Is a link that is relative to the current file.
  >For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:
  ```markdown
  [Contribution guidelines for this project](docs/CONTRIBUTING.md)
  ```
  >GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. The path of the link will be relative to the current file. Links starting with `/` will be relative to the repository root. You can use all relative link operands, such as `./` and `../`.
  
  >Relative links are easier for users who clone your repository. Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.

<br>

## 📌 Images
- `![ImageName](ImageURL)`
- display an image by adding `!` and wrapping the alt text in `[ ]`. Then wrap the link for the image in parentheses `()`.
```
![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)
```
![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

>GitHub supports embedding images into your issues, pull requests, discussions, comments and `.md` files. You can display an image from your repository, add a link to an online image, or upload an image. For more information, see "[Uploading assets](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#uploading-assets)."

Here are some examples for using [relative links](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#relative-links:~:text=Here%20are%20some%20examples%20for%20using%20relative%20links%20to%20display%20an%20image.) to display an image.

### [Specifying the theme an image is shown to](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#relative-links:~:text=Specifying%20the%20theme%20an%20image%20is%20shown%20to)

<br>

## 📌 Use HTML - `< >`
- You can use regular HTML in Markdown documents (depending on the parser that's being used).
So feel free to just input any valid HTML you like.

<br>

## 📌 Add Spacing - `---`
- If you want to add a horizontal line to divide up sections of a document, you can make one like this:
---

<br>

## 📌 Organizing Information with Tables

### 1. Creating a table
- You can create tables with pipes `|` and hyphens `-`.
- Hyphens are used to create each column's header, while pipes separate each column.
- You must include a blank line before your table in order for it to correctly render.
```markdown
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
```
**Output:**
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

>The pipes on either end of the table are optional.

- Cells can vary in width and do not need to be perfectly aligned within columns. There must be at least three hyphens in each column of the header row.

```markdown
| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |
```
**Output:**
| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |

### 2. Formatting content within your table
- You can use formatting such as links, inline code blocks, and text styling within your table:
```Markdown
| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |
```
**Output:**
| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |

- Align text to the left, right, or center of a column by including colons `:` to the left, right, or on both sides of the hyphens within the header row.
```Markdown
| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |
```
**Output:**
| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |

- To include a pipe `|` as content within your cell, use a `\` before the pipe:
```Markdown
| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |
```
**Output:**
| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |

<br>

## 📌 Ignoring Markdown Formatting
- You can tell GitHub to ignore (or escape) Markdown formatting by using `\` before the Markdown character.
```Markdown
Let's rename \*our-new-project\* to \*our-old-project\*.
```
**Output:** 

Let's rename \*our-new-project\* to \*our-old-project\*.

For more information, see Daring Fireball's "[Markdown Syntax](https://daringfireball.net/projects/markdown/syntax#backslash)."

<br>

## 📌 Hiding Content with Comments - `<!-- -->`
- You can tell GitHub to hide content from the rendered Markdown by placing the content in an *HTML comment*.
```Markdown
<!-- This content will not appear in the rendered Markdown -->
```

<br>

## 📌 Footnotes
- You can add footnotes to your content by using this bracket syntax:
```Markdown
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.
    This footnote also has been made with a different syntax using 4 spaces for new lines.
```

**Output:**

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.
    This footnote also has been made with a different syntax using 4 spaces for new lines.

<br>

---

### 🔗 Reference Links

[![FreeCodeCamp](https://img.shields.io/website?label=FreeCodeCamp&logo=FreeCodeCamp&style=for-the-badge&url=https%3A%2F%2Fwww.freecodecamp.org%2Fnews%2Fmarkdown-cheatsheet%2F)](https://www.freecodecamp.org/news/markdown-cheatsheet/) [![Github Docs](https://img.shields.io/website?label=Github%20Docs&logo=Github&logoColor=c9d1d9&style=for-the-badge&url=https%3A%2F%2Fdocs.github.com%2Fen%2Fget-started%2Fwriting-on-github%2Fgetting-started-with-writing-and-formatting-on-github%2Fbasic-writing-and-formatting-syntax)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)