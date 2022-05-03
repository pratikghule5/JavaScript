
1.What is server side css ?

**2.CSS Display properties?**
**1.static**\
The element is positioned according to the normal flow of the document. The top, right, bottom, left, and z-index properties have no effect. This is the default value.

**2.relative**\
The element is positioned according to the normal flow of the document, and then offset relative to itself based on the values of top, right, bottom, and left. The offset does not affect the position of any other elements; thus, the space given for the element in the page layout is the same as if position were static.

This value creates a new stacking context when the value of z-index is not auto. Its effect on table-*-group, table-row, table-column, table-cell, and table-caption elements is undefined.

**3.absolute**\
The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial containing block. Its final position is determined by the values of top, right, bottom, and left.

This value creates a new stacking context when the value of z-index is not auto. The margins of absolutely positioned boxes do not collapse with other margins.

**4.fixed**\
The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to the initial containing block established by the viewport, except when one of its ancestors has a transform, perspective, or filter property set to something other than none (see the CSS Transforms Spec), in which case that ancestor behaves as the containing block. (Note that there are browser inconsistencies with perspective and filter contributing to containing block formation.) Its final position is determined by the values of top, right, bottom, and left.

This value always creates a new stacking context. In printed documents, the element is placed in the same position on every page.

**5.sticky**\
The element is positioned according to the normal flow of the document, and then offset relative to its nearest scrolling ancestor and containing block (nearest block-level ancestor), including table-related elements, based on the values of top, right, bottom, and left. The offset does not affect the position of any other elements.

This value always creates a new stacking context. Note that a sticky element "sticks" to its nearest ancestor that has a "scrolling mechanism" (created when overflow is hidden, scroll, auto, or overlay), even if that ancestor isn't the nearest actually scrolling ancestor. This effectively inhibits any "sticky" behavior (see the GitHub issue on W3C CSSWG).

**2.Box model is css ?**\
The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content.\
**Content** - The content of the box, where text and images appear\
**Padding** - Clears an area around the content. The padding is transparent\
**Border** - A border that goes around the padding and content\
**Margin** - Clears an area outside the border. The margin is transparent\

The total width of an element should be calculated like this:

Total element width = width + left padding + right padding + left border + right border + left margin + right margin

The total height of an element should be calculated like this:

Total element height = height + top padding + bottom padding + top border + bottom border + top margin + bottom margin

3.psedo Classes?

**4. Border vs outline ?**

Border is created inside the element, where as outline is created outside the element. So border is computed along with the width and height of the element, while outline draws outside the element.

**5.Bootstrap breakpoints**
Breakpoints are the building blocks of responsive design. Use them to control when your layout can be adapted at a particular viewport or device size.

Use media queries to architect your CSS by breakpoint. Media queries are a feature of CSS that allow you to conditionally apply styles based on a set of browser and operating system parameters. We most commonly use min-width in our media queries.

Mobile first, responsive design is the goal. Bootstrap’s CSS aims to apply the bare minimum of styles to make a layout work at the smallest breakpoint, and then layers on styles to adjust that design for larger devices. This optimizes your CSS, improves rendering time, and provides a great experience for your visitors.


Breakpoint	Class infix	Dimensions
X-Small	None	<576px
Small	sm	≥576px
Medium	md	≥768px
Large	lg	≥992px
Extra large	xl	≥1200px
Extra extra large	xxl	≥1400px

- Media queries
- min-width
- max-width
 
**6.Grid vs flexbox.** 
The basic difference between CSS Grid Layout and CSS Flexbox Layout is that flexbox was designed for layout in one dimension - either a row or a column.\ Grid was designed for two-dimensional layout - rows, and columns at the same time.
