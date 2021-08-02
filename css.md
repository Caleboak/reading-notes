# What is CSS?
###  CSS describes how HTML elements are to be displayed on screen, paper, or in other media
### CSS can be used for very basic document text styling — for example changing the color and size of headings and links. It can be used to create layout — for example turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as animation.

## CSS Syntax
### CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example if you want your header read
> h1 {
    color: red;
    font-size: 5em;
}

- in the above example, h1 is the selector
- We then have a set of curly braces { }. Inside those will be one or more declarations, which take the form of property and value pairs. Before the colon, we have the property, and after the colon, the value

## How to add CSS - There are three ways to add CSS
- External CSS - With an external style sheet, you can change the look of an entire website by changing just one file. Each HTML page must include a reference to the external style sheet file inside the `<link>` element, inside the head section. Example: `<link rel="stylesheet" href="mystyle.css">`. Also they must be saved with a .css extension. For example `mystyle.css`

- Internal CSS - An internal style sheet may be used if one single HTML page has a unique style. The internal style is defined inside the `<style>` element, inside the head section. For example, `<head><style>body{color:red}</style></head>`

- Inline CSS - An inline style may be used to apply a unique style for a single element. To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property. For example, `<p style="color:red;">This is a paragraph.</p>`

*Note* : if the internal stylesheet and external style sheet are used together. The one defined first will get priority.

## Cascading order
### When there is more than one style specified for an HTML element, the priority will be as follows:
- Inline style (inside an HTML element)
- External and internal style sheets (in the head section)
- Browser default