## The Markdown language

Markdown is a lightweight markup language that you can use to add **formatting** elements to plain text documents. Created by [John Gruber](https://daringfireball.net/projects/markdown/) in ~2003~2004, Markdown is now one of the world’s most popular markup languages.

---

## Editing with Markdown output

The [CKEditor 5 WYSIWYG](https://ckeditor.com/) editor lets you use this flexible yet simple markup language in the GitHub flavor. The editor-produced Markdown output supports the most important features, like [links](https://ckeditor.com/), **different** kinds of _emphasis_, `inline code formatting` or code blocks:

```css
p {
text-align: center;
color: red;
}
```
Some Markdown text with <span style="color:#ffffff">some *blue* text</span>
<style>
r { color: Red }
o { color: Orange }
g { color: Green }
</style>
**My Bold Text, in red color.**{: style="color: red; opacity: 0.80;" }
# TODOs:

- <r>TODO:</r> Important thing to do
- <o>TODO:</o> Less important thing to do
- <g>DONE:</g> Breath deeply and improve karma
## Formatting blocks with Markdown
$${\color{red}Red}$$
## $\textcolor{yellow}{This\ is\ a\ Big\ Title}$
sdedsaf
# ${This\ is\ a\ {\color{red}Big}}\ Title$
Markdown can be used to create various block-level features, such as:

* Block quotes
* Headings
1. Heading 1
2. Heading 2
3. Heading 3
* Lists, including nested ones
* Numbered lists
* Bulleted lists
* To-do lists
```diff
- hello
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
## Support for tables in Markdown

![airwaysIcon](https://user-images.githubusercontent.com/121338960/209451471-eba18a9d-666a-4f54-94f3-b02bb07dec46.png)

Bear in mind that Markdown has only very basic support for tables, so things like table styles or merged cells will not work.

|   | Income | Revenue |
| --- | --- | --- |

| Walker 3 | $104.000 | 15% |
| Stroller | $12.000 | 10% |
| Runner | $97.500 | 15% |
