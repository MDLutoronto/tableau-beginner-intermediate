---
title: Creating Line Graphs
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
nav_order: 2
---

## Creating Line Graphs

1. Okay, let’s create a new visualization. Again, we need a new worksheet. **Click on the new worksheet icon at the bottom of the screen**. **Rename this one to “Line”.** 

2. We are going to create a line graph now, which is great to show trends over time. We are going to create a line graph of change in total profit over time. **Drag the Order Date variable** (**Dimensions**, under **Order**) **next to columns**. Next, **drag the Profit variable** (**Measures**) **next to rows**.

    ![Highlight of Order Date and Profit variables in the dimensions and measures sections as well as in pill form in the Columns and Rows sections respectively.]({{ '/assets/images/tableau_b2i_022.jpg' | relative_url }})

3. As we did before, **from the drop-down at the top change it from Standard to Entire View**.

4. It might be useful to see this graph broken down by sub-categories. **Drag the Sub-Category variable** (**Dimensions**, under **Product**) on to the **Colour** box in the **Marks** card. Tableau has used a qualitative colour palette scheme, assigning different colours to represent our sub-categories, but we do have a lot of them, so it is a bit overwhelming.

    ![Highlight of the Sub-Category variable in the Dimensions section as well as the Colour box in the Marks Card.]({{ '/assets/images/tableau_b2i_024.jpg' | relative_url }})

5. One way to simplify this would be to show a comparison between two particular sub-categories of interest. We can do this by **dragging the Sub-Category variable over to the Filters shelf.** Click on the **None** button to first clear the selections. Then select two sub-categories only – **pick Phones and Tables**. Now we are filtering the data to show only data for phones and tables. This tells a story that phones are increasing in profit, while tables are decreasing.

    ![The screen is pictured with the numbers 1 through 3, corresponding to the instructions above.]({{ '/assets/images/tableau_b2i_025.jpg' | relative_url }})

6. Another way we could do this would be to allow the user to filter it themselves based on what sub-categories they are interested in. To do that, **go back to Filters shelf, right click on the Sub-Category pill** and **pick Edit Filter**.

    ![Image displaying a drop-down menu from the Sub-Category Pill in the Filters Card with the item "Edit Filter..." highlighted.]({{ '/assets/images/tableau_b2i_026a.jpg' | relative_url }})

    Select the **All** button to re-select all the sub-categories and then click **OK**.

    ![An image displaying the Filter window with the "All" and "OK" buttons highlighted.]({{ '/assets/images/tableau_b2i_026b.jpg' | relative_url }})

    Then right click on the **Sub-Category** pill again, but this time select **Show Filter**.

    ![Image displaying a drop-down menu from the Sub-Category Pill in the Filters Card with the item "Show Filter" highlighted.]({{ '/assets/images/tableau_b2i_026c.jpg' | relative_url }})

    Now you can see the filters show up on the right. We can select or deselect as we like and the graph changes. (If you do not see the filters on the right, click on **Show Me** on the top right to close its options panel that might be blocking the view.)

    ![Image highlighting the resulting Filter to the right of the graph.]({{ '/assets/images/tableau_b2i_026d.jpg' | relative_url }})

7. To further help, the user read your graph, you could also add a highlighter. Go back to the **Filters** shelf, right click on the **Sub-Category** pill, but this time pick **Show Highlighter**.

    ![Image displaying a drop-down menu from the Sub-Category Pill in the Filters Card with the item "Show Highlighter" highlighted.]({{ '/assets/images/tableau_b2i_027a.jpg' | relative_url }})

    Now the **Highlight Sub-Category** box shows up on the right. The user can pick a sub-category and the graph emphasizes that sub-category. To try it out, make sure you have a few sub-categories showing first, then click on the **Highlight Sub-Category** search box to the see the list of sub-categories, and then hover over one sub-category’s name. You should see it emphasized in the graph.

    ![Image highlighting the resulting "Highlight Sub-Category" to the right of the graph.]({{ '/assets/images/tableau_b2i_027b.jpg' | relative_url }})

8. Right now it is showing the change in profit over time by years, but we can also change it to display more detail by quarters. One way to do this is to **click on the plus sign next to the Year (Order Date) pill** next to Columns.

    ![Image highlighting the plus sign beside the Year (Order Date) pill next to columns.]({{ '/assets/images/tableau_b2i_028a.jpg' | relative_url }})

    This subdivides each year by its quarters. You might see a pattern of end of year growth, cycling over each year, depending on what sub-categories you have selected.

    ![Image displaying the resulting line graph for each sub-quarter.]({{ '/assets/images/tableau_b2i_028b.jpg' | relative_url }})

9. Finally, let’s say you didn’t like these colours. Click on the **Colour** Box and select **Edit Colours**…

    ![Image displaying a dropdown menu from the Colour box in Marks Card. In the dropdown menu the button "Edit Colours..." is highlighted.]({{ '/assets/images/tableau_b2i_029a.jpg' | relative_url }})

    Here you can pick from a drop-down menu of various colour palettes, including a colour blind safe palette.

    ![Image displaying the Edit Colour Window with the Select Colour Palette dropdown menu highlighted.]({{ '/assets/images/tableau_b2i_029b.jpg' | relative_url }})

    Select one you like and click on **Assign Palette**. Then click on **OK**.

    ![Image displaying the Edit Colour Popup Window with the "Assign Palette" and "OK" buttons highlighted.]({{ '/assets/images/tableau_b2i_029c.jpg' | relative_url }})

10. **Give your graph the title “Quarterly Profit by Sub-Categories”**.

    ![Image displaying the resulting line graphs, subdivided by quarterly profit.]({{ '/assets/images/tableau_b2i_030.jpg' | relative_url }})