# EasyCSS
Making styles non-restrictive, simple, and comprehensive at the same time.

## How it works
This rep comes with 4 CSS files that all serve distinct purposes. They can be used in combination with your other CSS, but their purpose is to provide a foundation for styling a website and so they're perfectly fine to be used alone. <br>
- Flex.css
- Styles.css
- Media.css
- Reset.css

## How to use
Include this &lt;link&gt; tag in the header of your file:
```
<link href="https://cdn.jsdelivr.net/gh/natheerkhalil/easycss@master/all.css" rel="stylesheet">
```
Then, in the head, use the :root in a ``` <style> ``` tag to update the ``` --theme ``` variables (1-6) with colours of your choice. <br><br>
Alternatively, you can copy & paste the raw code of each CSS file and add them locally to have more control over the code.

## Reset.css
Reset.css does not contain class names and serves to remove all default styles from a webpage

## Flex.css
This file controls flex styles. The classes control the following flex attributes:

- Direction  ``` (fd) ``` 
- Wrap ```  (fw) ``` 
- Justify Content ```  (jc) ``` 
- Align Content ```  (ac) ``` 
- Align Items  ``` (ai) ``` 
- Order ```  (or) ``` 
- Grow ```  (gro) ``` 
- Basis ```  (bas) ``` 
- Shrink  ``` (shr) ``` 

The synax of a Flex.css class is: <br><br>
if Direction, Wrap, Align Content, Align Items: ``` _{id}-{value} ``` <br>
if Order, Grow, Basis, Shrink: ``` _{id}-{0 - 8 or 0 - 10) ``` <br> <br>
Order, Grow, Basis, Shrink use numbers as intensifiers. <br> Direction, Wrap, Align Content, Align Items use text representations of their possible values.

## Styles.css
This file controls the general shape, size, and colour of elements. It utilises 5 colours, each available in 10 shades (1-10):<br>
- ${\textsf{\color{rgb(204, 153, 0)}warn (yellow\)}}$
- ${\textsf{\color{rgb(204, 51, 51)}err (red\)}}$
- ${\textsf{\color{rgb(102, 153, 204)}info (blue\)}}$
- ${\textsf{\color{rgb(128, 128, 128)}grey (black to white\)}}$
- ${\textsf{\color{rgb(153, 204, 153)}succ (green\)}}$
<br>
There are also up to 6 theme colours that can be custom set. <br><br>
These colours are used for: <br>

- background ``` (bg) ```
- text colour ``` (txt) ```
- border colour ``` (bo) ```
- fill ``` (fi) ```
- background on hover ``` (hv) ```
- text on hover ``` (ht) ```
- fill on hover ``` (hfi) ```

  
<br>
Styles.css also utilises the following 7 sizes, from smallest to largest:

```
- xs
- sm
- md
- lg
- xl
- lx
- gl
```

<br> 
Not all classes contain all sizes. <br><br>

These sizes are used for: <br>

- break sizes ``` (br) ``` 
- max widths ```  (w) ``` 
- box shadows  ``` (shd) ``` 
- font sizes ```  (t) ``` 
- text alignment  ``` (t) ``` 
- margin auto direction ```  (m-auto) ``` 
- border radius  ``` (bd) ``` 
- padding ```  (pad) ``` 
- border width  ``` (bo) ``` 
<br>
The syntax of a Styles.css class is: <br>

if influenced by colour: ```  __{id}-{colour id}-{1 to 10 depending on desired colour shade} ```  <br>
if influenced by size:  ``` __{id}{size or value} ``` 

## Media.css
This file uses classes from Flex.css and Styles.css and allows you to decide on which viewpoint they should be used. <br><br>
The viewport has 6 sizes, from smallest to largest:

 ``` 
- xs
- sm
- md
- lg
- xl
- gl
 ``` 

The syntax of a Media.css class is  ``` _m-{size of viewport}-{class name as is from Flex or Styles} ``` 
