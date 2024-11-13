# Selctors
#### Selectors are the HTML elements to which CSS rules are applied
## Universal Selector
##### This selector will select elements of all types. 
```
* {
color: purple;
}
```
## Type Selectors
#### Only the specified element type is affected by the selector
```
div {
color: white;
}
```
#### will only select the element <div>
## Class Selectors
##### Selects elements in a specific class
```
<div class="alert-text">Please agree to our terms of service.</div>

```
```
.alert_text {
color: red;
}
```
#### selects the elements in the class, a period followed by the class name is used for syntax. white space is used to multiple classes. An element can belong to multiple classes. e.g-
```
class="alert-text severe-alert"
```
## ID Selectors
#### IDs are similar to classes, but one element can only belong to one ID.
```

<div id="title">My Awesome 90's Page</div>

```
```
#title {
  background-color: red;
}

```
## Grouping selectors
#### selectors can be grouped by using commas, which makes applying changes across various class and IDs easier
```
.read {
color: white;
background-color: black;
}

.unread {
color: white;
background-color: black;
}
```
#### is the same as 
```
.read,
.unread {
color: white;
background-color: black;
}

.read{}
.unread{}
```
## Chaining selectors
#### selectors can be chanined together to target very specific elements, for example:
```
<div>
  <div class="subsection header">Latest Posts</div>
  <p class="subsection" id="preview">
    This is where a preview for a post might go.
  </p>
</div>
```
#### the two elements can vbe selected individually by:
```
.subsection.header {
  color: red;
}

.subsection#preview {
  color: blue;
}
```
#### you can't chain more than one type selector because if we tried to chain together <div> and <p> we will get divp and the selector will try to look for a literal <divp> element. 
## Descendant combinator
```
.ancestor .contents {
}
 
```
#### would select the elements only if they are in the contents class AND if the content class is nested in the ancestor class. There is no limits to combinators and it doesn't matter how deep the class is nested.
# Properties
## Color and background-color
