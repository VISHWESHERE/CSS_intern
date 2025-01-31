CSS(Cascading style sheets)

--> Cascading style sheets is the styling language which provides styling option to html elements.
CSS can be applied to html in three ways they are:
1. Internal CSS
2. Inline CSS
3. External CSS

In the above three types of CSS Applicaiton techniques, Inline has more prority than any other techniques, then followed by internal and then Extenal.

Basically inline css in used to target single element.
Internal CSS is used for targetting single webpage.
External CSS is used for targetting multipage website.
__________________________________________________________________________________________________________________________________________________________

-->SELECTORS:
Selectors are used to mention a particular element, its is used to convey that this set of styling is used to apply for that particular element.

There are many types of CSS selectors:
1. can use element name directly, for example if you wanna mention <h1> element then you can just do this..
h1{
    apply style here
}

2. If you wanna provide a separate style to that particular element, then u can use class and id. 

<h1 class="heading" id="heading-main">Heading</h1>

They are attributes that can be applied inisde html tag. Difference between them is you can use same class name for different elements but id should be unique for each tag, i.e u can not use the same id to multiple elements. And if there are both class and id to a element and the style appiled is different then styling inside id has more priority.

3. * is used to mention the whole thing.(universal selector)
   * {
    font-size:"3rem";
   }

4. draggable :
draggable is the attribute that can be give to an html element.
for example:
p[draggable]{
    color:"red";
}

<p draggable="true">lorem</p>
here it applies the style to all the elements which has attribute draggable with value true.

5. Group selectors
they are used to apply the same style to group of elements.

selector, selector{
    style
}

6. child selector
they are kind of herarchial selector(only one level generation is accepted.)

selector(parent) > selector(child){
    style
}

7. Decendant
apply to a descendant of...

selector selector{
    style
}

8. chaining
apply where all selectors are true.(no space between selectors)

selectorselector{
    style
}

9. combine combiners:
selector selectorselectors{
    style
}

__________________________________________________________________________________________________________________________________________________________

--> POSITIONING

Positioning is setting the position of particular element.
there are mainly 5 types of positioning, they are:
1. Static Positioning:
It is the normal positioning of the element.
2. Relative Positioning: 
By using this positioning the element will be positioned next to the nearest ancestor element.
3. Absolute Positioning:
By applying this positioning the element is positioned relative of the top of the page (top left corner and enable to scroll)
4. Fixed Positioning: 
By applying this positioning the element is positioned relative of the top of the page (top left corner and not able to scroll)
5. Sticky
This positioning will make the element to be sticked to a place usally used for navbar.

__________________________________________________________________________________________________________________________________________________________

--> span tag is used to style a particular part of the element.
<h1>Hello everyone, this is <span>vishweshwar</span></h1>

__________________________________________________________________________________________________________________________________________________________

some of the attributes :
1. display: "none"; (will disappear)
values: inline, inline-block, block
2. css-float
float: left; (wrapping text around img)
clear : left; (counter style to above float.)

__________________________________________________________________________________________________________________________________________________________

RESPONSIVENESS:

So, to make the website responsive there are 4 ways and they are 
1. Media queries
2. CSS grid
3. CSS flexbox
4. external frame work
 
_____________________________________________________________________________

FLEX BOX:

Display:"flex";(to initiate flex box start telling that u are going to using flex box by this attribute)

     ATTRIBUTES               VALUES

1. justify-content        flex-start
                          flex-end  
                          center
                          space-between
                          space-around
                          space-evenly

2. align-items            flex-start
                          flex-end
                          center
                          baseline
                          stretch(default)

3. flex-direction         row(default)
                          column
                          column-reverse

4. order                  ... -3 -2 -1 0 1 2 3 ...

5. align-self             aligns a flex item along the cross axis, overriding the align items value.
                          flex-start
                          flex-end
                          center
                          baseline
                          stretch
                        
6. flex-wrap              specifies whether flex items are forced on a single line or can be wrapped on multiple lines.
                          nowrap(default)
                          wrap
                          wrap-reverse 

7. flex-flow:             short hand property for flex-direction and flex-wrap

8. align-content          aligns a flex container's lines with in the flex container when there is extra space on the cross axis.
                          flex-start
                          flex-end
                          center
                          space-between
                          space-around
                          space-evenly
                          strech(default)  

Game to lear flex box: flexbox froggy 

__________________________________________________________________________________________________________________________________________________________

GRID SYSTEM

flexbox is used to do one dimensional layouts.
grid system is used to do two dimesional layouts.

to make the grid first we need to mention :

display:"grid";

The idea behind the grid system is to make a grid, and insert the elements in those cells present in the grid.

so first we have to create a design how our page should look like and then create that exact design on the webpage using grid attributes and then insert respective elements as per the design.

firstly give the height and width of the container.

To create grid design we should use the following attributes:

grid-template-rows: 140px 140px 45px 45px;  -----|
                                                 |---> grid-template: <grid-temp-row> / <grid-temp-column>
grid-template-columns: 100px 260px 20px;    -----|

grid-column: span3;
grid-column: span2;
grid-column-start: span2;
grid-column-start: auto;
order: 1;

instead of these below attibutes you write these four attributes using short hand ( grid-area: <row-start> / <column-start> / <row-end> / <column-end> )
grid-column-start: 1;
grid-column-end:3;
grid-row-start:2;
grid-row-end:3;

advantages of the grid:
we can overlay an element on another element, where as in flexbox we cant.
to apply opacity in the colour represents the number of percentage after the hexcode(colour code).
for example if hte colour is #ffffff and u want opacity of 50% then place 50 at the end of the colour code, #ffffff50

__________________________________________________________________________________________________________________________________________________________

