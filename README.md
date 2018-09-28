# css flexbox

1. Example on using flexbox.
2. Parent level apis for `display:flex`

##### Display Flex parent level properties

1. flex-flow,
this contains flex-direction & flex-wrap.

Example:
```bash
flex-flow: row wrap;
```
flex-direction functions by Main Axis vs. Cross Axis concept
```bash
# flex-direction: row
main axis starts on the Left--->
                            |
                            |
                            cross axis
```

```bash
# flex-direction: row-reverse
<-----| Main axis starts from Right
      |
      |
      cross axis
```

```bash
# flex-direction: column
|---->Cross axis starts from Right
|                          
|                            
Main Axis heads DOWN
```

```bash
# flex-direction: column-reverse
Main Axis heads UP^
|
|                          
|---->Cross axis starts from Right        
```
#


2. align-items: adjusted by cross axis

Only reffers to the position of the items relating to the cross-axis
So, if `flex-direction: column` then it's starting point is left ---> right.
And if `flex-direction: row` then the cross axis starts top ---> bottom.

#

3. justify-content: adjusted by main-axis
So if `flex-direction: row` & `justify-content: center`, then the content would be centered coming from the left.
#

4. align-content

