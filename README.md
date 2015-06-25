# Week 1 Homework

## Part 0: Getting Started

The first step before doing any work will always be to **fork** and then **clone** a repository.

Please follow [the guide to Getting Started With GitHub](https://gist.github.com/rbetina/22186869342fce3bec6b), and use it to fork and clone this repository that you are reading right now. You will always follow this same process to start and submit your work.

**Note:** A couple of you were unable to download the GitHub Desktop App for a Mac OS X version less than 10.9. If so, please send me an email and I'll reply with a solution.

Next, [follow this guide to tweaking your Sublime](https://gist.github.com/rbetina/d07e134223fde2ca4299) to make your life much easier as we move forward.

## Part 1: Review What We Did In Class

In the folder `1_roster`, you'll recognize some files from class. Review each starting point and target, and ask questions on the forum about things that are still fuzzy. In particular,

### HTML Tables

An important element in HTML is `<table>`.

`<table>`s in HTML are used to represent two dimensional data. A simple table looks like this:

    <table>
      <tr>
        <th>First</th>
        <th>Last</th>
      </tr>
      <tr>
        <td>John</td>
        <td>Doe</td>
      </tr>
      <tr>
        <td>Jane</td>
        <td>Doe</td>
      </tr>
    </table>

which would produce this:

<table>
  <tr>
    <th>First</th>
    <th>Last</th>
  </tr>
  <tr>
    <td>John</td>
    <td>Doe</td>
  </tr>
  <tr>
    <td>Jane</td>
    <td>Doe</td>
  </tr>
</table>

The things to keep in mind about tables are:

 - Every piece of data must reside within a cell, a `<td>` element (or maybe a `<th>` element if it's a heading).
 - Every `<td>` or `<th>` element must reside within a row, a `<tr>` element.
 - Every `<tr>` must have the same number of cells, or things get out of whack.

Despite this last rule, you can, however, "merge" cells using the `colspan` and `rowspan` attributes:

    <table>
      <tr>
        <th colspan="2">People</th>
      </tr>
      <tr>
        <td>John</td>
        <td>Doe</td>
      </tr>
      <tr>
        <td>Jane</td>
        <td>Doe</td>
      </tr>
    </table>

produces:

<table>
  <tr>
    <th colspan="2">People</th>
  </tr>
  <tr>
    <td>John</td>
    <td>Doe</td>
  </tr>
  <tr>
    <td>Jane</td>
    <td>Doe</td>
  </tr>
</table>

You can see that we've merged two cells in the first row together; the `colspan="2"` on the first cell ensures that we don't violate the "every `<tr>` must have the same number of cells" rule.

Similarly, you can merge cells vertically:

    <table>
      <tr>
        <th rowspan="2">People</th>
        <td>John</td>
        <td>Doe</td>
      </tr>
      <tr>
        <td>Jane</td>
        <td>Doe</td>
      </tr>
    </table>

produces:

<table>
  <tr>
    <th rowspan="2">People</th>
    <td>John</td>
    <td>Doe</td>
  </tr>
  <tr>
    <td>Jane</td>
    <td>Doe</td>
  </tr>
</table>

Now, each row has three cells. The second row doesn't look like it at first glance, but the first cell in the first row is spanning down across two rows, so the second row really does have three cells.

### Using Tables For Positioning

Can you see how you could use a `<table>` to achieve horizontal positioning? In the real world, we would never do this; but, for learning purposes, do it now to achieve the three-column layout we want for our roster.

# Part 2: Chessboard

 - Open `2_chessboard/chessboard_styles.css` in Sublime.
 - Open `2_chessboard/chessboard_start.html` in Sublime and Chrome.
 - Open `2_chessboard/solution/chessboard_target.html` in Chrome.
 - Write CSS rules in `2_chessboard/chessboard_styles.css` until your document matches the target. I've added some comments in that file with links to references that might be useful.
 
# Part 3: Landing Page with table

 - Open `3_landing_with_table/landing_with_table_start.html` in Sublime and Chrome.
 - Open `3_landing_with_table/solution/landing_with_table_target.html` in Chrome.
 - Edit the starting point until it looks like the target.

# Part 4: Canvas Positioning

Let's say we get hired to create an HTML page that looks like [this](https://en.wikipedia.org/wiki/Business_Model_Canvas#/media/File:Business_Model_Canvas.png).

We'll work on it in two stages: first, laying out the positioning of the page, and then fine tuning the styling.

- Open `4_canvas_positioning/canvas_positioning_start.html` in Sublime and Chrome.
- Open `4_canvas_positioning/solution/canvas_positioning_target.html` in Chrome.
- I've already stubbed out some content in the starting point. Use a `<table>` to roughly position things until your document looks like the target.

# Part 5: Canvas Styling

- Open `5_canvas_styling/canvas_styling_start.html` in Sublime and Chrome.
- Open `5_canvas_styling/solution/canvas_styling_target.html` in Chrome.
- In this starting point, I've already positioned and fleshed out the content. I've also added some classes on to elements. Your job is to write CSS rules to make the document more visually appealing. Try to make it look as much like the target as possible. It doesn't have to be pixel-perfect.

# Part 6: Optional Readings

- [Butterick's Typography In Ten Minutes](http://practicaltypography.com/typography-in-ten-minutes.html)
- [7 Rules For Creating Gorgeous UI](https://medium.com/@erikdkennedy/7-rules-for-creating-gorgeous-ui-part-1-559d4e805cda)
- [Paul Graham's "How To Get Startup Ideas"](http://paulgraham.com/startupideas.html)
