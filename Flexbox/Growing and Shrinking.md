# Flex Shorthand
#### just writing 'flex' is shorthand for flex-grow, flex-shrink and flex-basis. 
```
div {
flex: 1;
}
```
#### equates to flex-grow: 1, flex-shrink: 1, flex-basis: 0.
# Flex-grow
#### determines the growth rate. if one div has "flex: 1" and another has "flex: 2", then the second div will grow to twice the size of others.
# Flex-shrink
#### determines the shrink factor if the flex items are larger than  the parent container. 1 means they will shrink evenly and 0 means the element won't shrink at all.
# Flex-basis
#### determines the baseline size. auto means its main size is determined on the width/height property. 0 means it's given zero width and height and grows accordingly.
