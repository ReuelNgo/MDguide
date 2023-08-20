## 1. Syntax Fundamentals: Mastering the foundational elements of Markdown, from headers and lists to links and images.

Since MD does not support commenets, Comments will be written as shown below:
- this is a comment

### headings

To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three (h3), use three number signs (e.g., ### My Header).

Alternate syntax
Alternatively, on the line below the text, add any number of == characters for heading level 1 or -- characters for heading level 2.

- Heading level 1
- ===============
Will give you

Heading level 1
=====

#### Heading best practices
markdown apps don't agree on how to handle missing spaces between number signs (#). Therefore, always put a space in the number sign and header
- DO: # Header
- DONT: #Header

## Paragraph
To create paragraphs, use a blank line to separate one or more lines of text.
The best practice is not to use **spaces** or **tabs** in front of your paragraphs.
Keep lines left aligned.

## line breaks
To make line breaks, end a line with 2 or more spaces. This is known as **trailing whitespace**.   
Readability is still bad though, and many people intentionally put 2 spaces after the nextline.  
Therefore, if your applicaiton suports HTML, try to use the br HTML tag
- The one we should avoid is using backslash (\). But not markdown applications support this.

## Emphasis
To bold text, add (**) or (__) before and after text.
However, try not to use underscores as some applications don't agree how to handle this.

Italics can be done by using (*) or (_)
However, try not to use underscores as some applications don't agree how to handle this.

To bold and italics at the same time, use (***) before and after text.

## Block Quotes

To create a blockquote, add > infront of a paragraph

    > Dorothy followed her through many of the beautiful rooms in her castle.

If you need to have multiple paragraphs, make sure you have > at the beginning of each line for the paragraph.

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

Lastly, if you need to have nested blockquotes, put >>.

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

You can also have blockquotes with other elements

    > ### The quarterly results look great!
    > 
    > - Revenue increased by 55%
    > - Profits were higher than **ever**!

For blockquotes, try to put a blankline before and after a blockquote.

## lists

Ordered lists - just put x. , don't put x)

    1. Number 1

    2. Number 2

    3. Number 3

Undordered lists - add a (-), (*), or (+). Indent one or more itesm to create a nested list.

If you need to start unordered list items with numbers - you can use a (\) to escape the period. Some editors don't need this.

    1. 1990 was the year i was born.

Adding elements in lists
To add another element in a list, make sure you indent the element 4 spaces or one tab

* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third list item.

Or

* This is the first list item.
* Here's the second list item.

    > A blockquote would look great below the second list item.

* And here's the third list item.

### Code blocks in a list
These are normally indented 4 spaces or 1 tab. When they're in a list, indent them 8 spaces or 2 tabs


1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.

### images in a list

1. You can even put gifs here. Not sure if this is always supported but who cares.
2. Marvel at its beauty.

    ![Mashle](https://64.media.tumblr.com/bb5e274e952ad8d7088208b88adcd0b9/8b10ded8c264a556-23/s540x810/542cf0cfcc30c5f3f3c03f198755bf372b64ea7c.gifv)

3. watch the anime. Mashle: Magic and Muscles

## list within list
1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

## code

To denote code, enclose it in backticks (`).

type in `get`.
To escape backticks, use another backtick.

To create code blocks, indent everyline with 4 spaces or 1 tab

    This is some code
    code should be written in code blocks
    Code blocks allow you to copy code.
    ### Headers and other markdown elements do not work in code blocks

## Horizontal rules
To create a horizontal line
    ***, ---, ____ on a line by themselves
***

## links

To createa a link, enclose the link text in brackets and follow up with a url in parenthses  
e.g. (  [url text here](insert url link here) )  
    My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

## Adding titles

you can add a title for a link aka tooltip. To add a title, enclose it with quotation marks after the url.

My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").

## urls and emails

To turn a url or email into a link, enclose it with angle brackets (<)  

<email@mail.com>  

## Formatting links
To emphasize links, add asterisks before and after the brackets and parentheses. To denote links as code, add backticks in the brackets.

I love **[Google](www.google.com)**  
I love *[Bing](www.bing.com)* as I'm a microsoft employee.  

For links, markdown might not be able to handle spaces in urls, so replace any spaces in urls with "20%".

## images
To add an image, add (!) followed by alt text in brackets, and the url path to the image asset in parenthesis  
    ![Image alt text here](file path or url to image here "Optional image title here")

![Truck Kun getting rekt](https://i.redd.it/2p6vqu77b6321.jpg "Truck-kun getting destroyed")

### Linking images
yea, this just means when a user hovers over a image, they get taken to another page  

    [![alt text](filepath "Image title")](Image url)

[![Truck Kun getting rekt](https://i.redd.it/2p6vqu77b6321.jpg "Truck-kun getting destroyed")](www.google.com)
