# Object Literal

- object literal is the easiest and most popular way to create objects

## DOM (Document Object Model)

- The DOM is neither part of HTML, nor part of JavaScript. DOM accesses a separate set of rules

- DOM trees have four types of nodes, document, element, attribute and text. 

## Fundamental Data Types

- Document: When a member returns an object of type document (e.g., the ownerDocument property of an element returns the document to which it belongs), this object is the root document object itself. The DOM document Reference chapter describes the document object.

- Node: Every object located within a document is a node of some kind. In an HTML document, an object can be an element node but also a text node or attribute node.

- Element: The element type is based on node. It refers to an element or a node of type element returned by a member of the DOM API. Rather than saying, for example, that the `document.createElement()` method returns an object reference to a node, we just say that this method returns the element that has just been created in the DOM. element objects implement the DOM Element interface and also the more basic Node interface, both of which are included together in this reference. In an HTML document, elements are further enhanced by the HTML DOM API's HTMLElement interface as well as other interfaces describing capabilities of specific kinds of elements (for instance, HTMLTableElement for `<table>` elements).

- Node List: A nodeList is an array of elements, like the kind that is returned by the method document.querySelectorAll(). Items in a nodeList are accessed by index in either of two ways:
list.item(1)
list[1]
These two are equivalent. In the first, item() is the single method on the nodeList object. The latter uses the typical array syntax to fetch the second item in the list.

- Attr: When an attribute is returned by a member (e.g., by the createAttribute() method), it is an object reference that exposes a special (albeit small) interface for attributes. Attributes are nodes in the DOM just like elements are, though you may rarely use them as such.

- NamedNodMap: A namedNodeMap is like an array, but the items are accessed by name or index, though this latter case is merely a convenience for enumeration, as they are in no particular order in the list. A namedNodeMap has an item() method for this purpose, and you can also add and remove items from a namedNodeMap.

Above was taken from https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction