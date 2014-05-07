![DOM-to-XHTML](https://raw.githubusercontent.com/stimpy77/xhtml.js/master/dom-to-xhtml.png "xhtml.js DOM-to-XHTML")

xhtml.js
========

Cleans up extracted HTML to produce formatted XHTML

This is a migration of the same project from https://xhtmljs.codeplex.com which was created in 2008.

---

XHTMLJS is a Javascript library that converts a web browser's pre-parsed DOM element into valid XHTML. This attempts to resolve the inadequacies of ELEMENT.innerHTML by providing innerXTML() and outerXHTML() to the web developer.

Developers often need XHTML-compliant HTML markup when they fetch DOM elements' innerHTML. Since the W3C hasn't standardized on this property (for whatever reason) the browsers have been inconsistent in their approaches to innerHTML. Firefox doesn't put the trailing slash in `<br>` tags, for instance, while Internet Explorer shows tags in all-caps and strips the quotation marks from single-word attributes. 

This project is an attempt to alleviate the problem by creating innerXHTML() and outerXHTML() functions in Javascript. 

The original intent was to add innerXHTML() and outerXHTML() to the prototype of Element, but Internet Explorer doesn't expose a prototype for DOM elements. The innerXHTML() and outerXHTML() functions are implemented anyway, and are added to the Element prototype for browsers that support Element prototypes. The function xhtml() for innerXHTML() equivalence is also added to jQuery. 
