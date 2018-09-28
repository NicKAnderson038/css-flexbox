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
`flex-direction`: functions by Main Axis vs. Cross Axis concept
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
Main Axis heads TOP--->BOTTOM
```

```bash
# flex-direction: column-reverse
Main Axis heads BOTTOM--->UP
|
|                          
|---->Cross axis starts from Right        
```
#


2. `align-items`: adjusted by cross axis So if `flex-direction: row` & `alight-items: center`, then the content would be centered coming from the top ---> bottom.

#

3. `justify-content`: adjusted by main-axis
So if `flex-direction: row` & `justify-content: center`, then the content would be centered coming from the left ---> center.

#

4. `align-content`: defines extra space characteristics based on cross-axis.
All these `<div>` will have there blank spaces adjusted. So `align-content:space-between` would adjust the space (on view resizing) to keep the `<div>` sizes by forcing them to the ends so a large amount of white space would appear between them.

