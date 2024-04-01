# Assignment-12

---
title: "R Markdown"
author: "Yamini"
date: "2023-04-03"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

# Headers

Headers in R Markdown are used to create headings and subheadings within a document. They provide a way to organize and structure your content by indicating the hierarchy of your sections.

Headers are created using the "\#" symbol, and there are six levels of headers. A single "\#" symbol creates a level 1 heading, two "\#" symbols create a level 2 heading, and so on up to level 6.

Here is an example of how to create headers in R Markdown:

# Level 1 Heading

## Level 2 Heading

### Level 3 Heading

#### Level 4 Heading

##### Level 5 Heading

###### Level 6 Heading

This will create six different levels of headers, each with a different font size and style to indicate their hierarchy. You can also add additional formatting to your headers, such as bold or italic text, by using Markdown syntax within the header text. For example:

# **Bold** Level 1 Heading

## *Italic* Level 2 Heading

### Level 3 Heading with **bold** and *italic* text

This will create headers with both bold and italic text, as well as different font sizes and styles to indicate their hierarchy.

# Lists

Lists are a great way to organize information in R Markdown documents. There are two types of lists: ordered and unordered.

An unordered list is a list of items that does not have a specific order or ranking. Items in an unordered list are marked with a bullet point, which can be an asterisk, a hyphen, or a plus sign. Here's an example of an unordered list:

-   Item 1
-   Item 2
-   Item 3 This will create a list with three items, each marked with a bullet point.

An ordered list is a list of items that has a specific order or ranking. Items in an ordered list are numbered in order, starting with 1. Here's an example of an ordered list:

1.  First item
2.  Second item
3.  Third item This will create a list with three items, each numbered in order.

You can also create nested lists, which are lists that are indented to show a hierarchical relationship between items. Here's an example of a nested list:

-   Item 1
    -   Sub-item 1a
    -   Sub-item 1b
-   Item 2
    -   Sub-item 2a
    -   Sub-item 2b This will create a list with two main items, each with two sub-items.

You can also mix and match ordered and unordered lists, and you can add additional formatting to your lists, such as bold or italic text. Here's an example:

-   **Bold** item 1
-   *Italic* item 2
    1.  First sub-item
    2.  Second sub-item
-   Item 3 This will create a list with three items, the first with bold text, the second with italic text and two sub-items that are numbered in order, and the third with no additional formatting.

# Links and Images

Links and images are powerful tools for enhancing the content of R Markdown documents. They can be used to provide additional context, reference sources, or simply make your document more visually appealing.

Links To add a link to your R Markdown document, you use the following syntax:

    [link text](url)

Here, "link text" is the text that you want to display as the link, and "url" is the URL that the link should point to. For example:

[Click here to go to Google](https://www.google.com)

This creates a hyperlink with the text "Click here to go to Google" that will take the user to the Google homepage when clicked.

You can also add a title to your link by including it in quotes after the URL:

[Click here to go to Google](https://www.google.com "Google Homepage")

This creates the same hyperlink as before, but with the title "Google Homepage".

Images To add an image to your R Markdown document, you use the following syntax:

    ![](url)

Here, "url" is the URL of the image that you want to display. For example:

![](https://cdn.vox-cdn.com/thumbor/I8dQfh6H7S3fb9JR7wvJETsHOLA=/0x0:3172x4828/1220x813/filters:focal(1255x1045:1761x1551):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/50629459/usa-today-8118829.0.jpg)

This creates an image that displays the USF's Rocky the Bull.

You can also add a caption to your image by including it in square brackets before the URL:

![USF's Rocky the Bull](https://cdn.vox-cdn.com/thumbor/I8dQfh6H7S3fb9JR7wvJETsHOLA=/0x0:3172x4828/1220x813/filters:focal(1255x1045:1761x1551):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/50629459/usa-today-8118829.0.jpg "USF's Rocky the Bull")

This creates the same image as before, but with the caption "USF's Rocky the Bull" displayed beneath it.

In addition to URLs, you can also use local file paths to display images that are stored on your computer:

    ![](file_path)

Here, "file_path" is the path to the image file on your computer. For example:

![](images/download.jpeg)

This displays an image of a ducati bike photo that is stored in the "Pictures" folder in the user's home directory.

# LaTeX Expressions in R

LaTeX is a powerful typesetting language that can be used in R Markdown documents to create mathematical expressions and equations.

To include a LaTeX expression in your R Markdown document, you need to surround it with "\$" symbols. For example:

The formula for the area of a circle is $\pi r^2$. This will create an inline LaTeX expression that displays the formula for the area of a circle, with the "r" variable raised to the power of 2.

You can also use double "\$\$" symbols to create a display-style LaTeX equation:

    $$
    \int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
    $$

$$
\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
$$

This will create a display-style LaTeX equation that calculates the definite integral of the function e^{-x^2} from 0 to infinity, which is equal to the square root of pi divided by 2.

LaTeX offers a wide range of mathematical symbols and expressions, including fractions, integrals, summations, matrices, and more. Here are a few more examples of LaTeX expressions that can be used in R Markdown:

    The formula for the slope of a line is $m = \frac{y_2 - y_1}{x_2 - x_1}$.

    The sum of the first 10 positive integers is $\sum_{n=1}^{10} n = 55$.

    The determinant of a 2x2 matrix is given by $|A| = \begin{vmatrix} a & b \\ c & d \end{vmatrix} = ad - bc$.

The formula for the slope of a line is $m = \frac{y_2 - y_1}{x_2 - x_1}$.

The sum of the first 10 positive integers is $\sum_{n=1}^{10} n = 55$.

The determinant of a 2x2 matrix is given by $|A| = \begin{vmatrix} a & b \\ c & d \end{vmatrix} = ad - bc$.

These examples demonstrate some of the many possibilities for using LaTeX expressions to create mathematical content in R Markdown documents.

# Code Blocks

Code blocks can be used to display larger sections of code within your document. To create a code block, you simply surround your code with three backticks (\`\`\`). For example:

```{r}
x <- 1:10 
y <- x^2 
plot(x, y)
```

This will create a code block that displays R code for creating a plot of the values in the "x" and "y" vectors.

You can also specify the language of the code block by adding the language identifier after the opening backticks. This can be useful when working with multiple programming languages within the same document:

```{python}
import matplotlib.pyplot as plt
x = range(10) 
y = [i**2 for i in x] 
plt.plot(x,y)
```

This will create a code block that displays Python code for creating a similar plot.

## Inline Code

Inline code can be used to display small sections of code or to reference variables and objects within your document. To create inline code, you simply surround your code with a single backtick (\`). For example:

```{r}
x <- 5  # radius of a circle
```

For a circle with the radius `r x`, its area is `r pi * x^2`.
