---
title: Creating Highlight Tables
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
nav_order: 4
---

## Creating Highlight Tables

1. Next, let’s change gears here a bit and look at creating a highlight table. It is a hybrid between a visualization and a table. Tables can be very useful when you need to look up a value and see both precise values and summary stats. To add a visualization piece, you can shade the background of various cells to highlight cells of interest – perhaps the values are too high or low. Let’s create one showing sales by sub-category, broken down by region.

2. Again, first we need a new worksheet. **Click on the new worksheet icon at the bottom of the screen. Let’s rename this one to “Sales Table”.** 

3. **Drag the Sub-category variable** (**Dimensions,** under **Product**) **next to rows** and **the Region variable** (**Dimensions**) **next to columns**.

    ![Highlight of Sub-category and Region variables in the Dimensions section as well as in pill form in the Columns and Rows sections respectively.]({{ '/assets/images/tableau_b2i_043a.jpg' | relative_url }})

    Then **drag the Sales variable** (**Measures**) to the **Text** box on the **Marks** card.

    ![Highlight of the Sales variable in the Measure section as well as the Text box in the Marks card.]({{ '/assets/images/tableau_b2i_043b.jpg' | relative_url }})

4. To make it a highlight table, we need to add colour, so **drag Sales again**, this time to the **Colour** box on the **Marks** card. To make the cells shaded, from the **Marks card drop-down**, **select Square**.

    ![Marks card drop-down menu with the Square menu-item highlighted.]({{ '/assets/images/tableau_b2i_044a.jpg' | relative_url }})

    Now you can easily see for example that Chairs and Phones make a lot of sales in the East and West regions.

    ![The resulting highlight table with cells colour-coded by sales.]({{ '/assets/images/tableau_b2i_044b.jpg' | relative_url }})

5. We can also add grand totals by region to add more information to our table. Go to the **Analysis menu**, and **select Totals**, and then **Show Column Grand Totals**.

    ![Image displaying the Analysis dropdown menu. In the master dropdown menu ‘Totals' is highlighted. From this selection a sub-drop down menu is shown with the option ‘Select Column Grand Totals'' highlighted.]({{ '/assets/images/tableau_b2i_045.jpg' | relative_url }})

6. Let’s quickly create one more highlight table, as we will use it later in the activity. But, this time, make a table show profit instead of sales.

7. Again, we need a new worksheet. **Click on the new worksheet icon at the bottom of the screen. Let’s rename this one to “Profit Table”.** 

8. **Drag the Sub-category variable** (**Dimensions,** under **Order**) **next to rows** and **the Region variable** (**Dimensions**) **next to columns**. Then **drag the Profit variable** (**Measures**) to the **Text** box on the **Marks** card.

9. Then **drag Profit again**, this time to **Colour** box on the **Marks** card, and from the **Marks card drop-down**, **select Square**. From this table, you can easily see for example that Tables are causing a loss in the East. Add Column Grand Totals here as well, by going to the **Analysis menu**, and **selecting Totals**, and then **Show Column Grand Totals**.

    ![The resulting highlights Profit table.]({{ '/assets/images/tableau_b2i_049.jpg' | relative_url }})
