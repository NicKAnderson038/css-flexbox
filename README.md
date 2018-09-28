# css flexbox

1. Example on using flexbox.
2. Parent level apis for `display:flex`

##### Display Flex parent level properties

1. `flex-flow`
this contains flex-direction & flex-wrap.

Example:
```bash
flex-flow: row wrap;
```
`flex-direction`: functions by ** Main Axis vs. Cross Axis ** concept
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
|---->Cross axis Left--->Right
|                          
|                            
Main Axis heads TOP--->BOTTOM
```

```bash
# flex-direction: column-reverse
Main Axis heads BOTTOM--->UP
|
|                          
|---->Cross axis Left--->Right       
```
#


2. `align-items`: adjusted by cross axis So if `flex-direction: row` & `alight-items: center`, then the content would be centered coming from the top ---> bottom.

#

3. `justify-content`: adjusted by main-axis
So if `flex-direction: row` & `justify-content: center`, then the content would be centered coming from the left ---> center.

#

4. `align-content`: defines extra space characteristics based on cross-axis.
All these `<div>` will have there blank spaces adjusted. So `align-content:space-between` would adjust the space (on view resizing) to keep the `<div>` sizes by forcing them to the ends so a large amount of white space would appear between them.

#

##### Display Flex items **single "div"

*** All these child properties are affected by flex-flow!

1. `order` property
Ex. `order:1` on the first div would position it last. All other divs are treated as `order:0` by default.

#

2. `align-self` property - based on parent cross-axis
Ex. `flex-direction: row` in parent and set `align-self:flex-start` on the child div would set it at the top of the page.

#

2. `flex` - contains 3 properties (`flex-grow`, `flex-shrink`, `flex-basis`)
```bash
# flex default setting
# 0 = flex-grow
# 1 = flex-shrink
# auto = flex-basis

flex: 0 1 auto;
```
- flex-grow will grow will increase the width to fill the whole page.
- And if the first div is set to `flex-grow:1` and the second div is set to `flex-grow:2` They will both grow but at a 2:1 ratio.