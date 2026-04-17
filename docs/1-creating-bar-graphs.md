---
title: Creating Bar Graphs
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
nav_order: 1
---

## Creating Bar Graphs

1. Start by **opening up *Tableau Desktop***.

2. We are going to start with a built-in dataset. Under **Saved Data Sources**, **select Sample - Superstore.** 

    **![Tableau's connect menu. The option 'Sample-Superstore' is highlighted.]({{ '/assets/images/tableau_b2i_002.JPG' | relative_url }})**

3. On the left you can see our variables listed, categorized by Dimensions and Measures. Dimensions are roughly qualitative data and measures are roughly quantitative data.

    ![The Dimensions section at the top of the Side Bar and the Measures section directly below it, both highlighted.]({{ '/assets/images/tableau_b2i_003a.JPG' | relative_url }})

    The centre area is where you’ll be dragging and dropping your variables on to different sections, such as rows and columns, or to vary mark characteristics such as colour or size by your variable, or filtering by a variable. In terms of Tableau terminology, those areas that say filters or pages are called shelves, the marks area is called a card and when the variables are showing up in those areas, they are called pills, as they are shaped like a pill.

    ![The Filters and Marks sections are highlighted, located to the left of the sheet. The Columns and Rows sections are also highlighted, located at the top of the sheet.]({{ '/assets/images/tableau_b2i_003b.JPG' | relative_url }})

4. Okay, we have loaded in some data about a fictional superstore, so let’s start by creating some visualizations that are used to make comparisons. Let’s start by making a simple bar graph. To keep track of all the visualizations we are going to create, let’s rename our sheets as we go. **Right-click on Sheet 1** at the bottom, **select rename**.

    ![Image displaying a menu emerging from the Sheet 1 tab at the bottom of the application. In the menu the item 'Rename' is highlighted.]({{ '/assets/images/tableau_b2i_004a.jpg' | relative_url }})

    **Give it the name “Sales Bar”** and **press Enter.** 

    ![The result of renaming the new sheet to “Sales Bar”.]({{ '/assets/images/tableau_b2i_004b.jpg' | relative_url }})

5. We are going to create a horizontal bar graph to compare the amount of sales for different sub-categories of products, with sub-categories along the y-axis and sales along the x-axis. Bar graphs are great for comparing categories. So **drag the Sales variable** (in the **Measures** section) **next to columns** and the **Sub-category variable** (in the **Dimensions** section, under **Product**) **next to rows**.

    ![Highlight of Sales and Sub-Category variables in their original dimensions and measures sectopms as well as in pill form in the Columns and Rows sections respectively.]({{ '/assets/images/tableau_b2i_005.JPG' | relative_url }})

6. You can see that when we dragged Sales, it automatically summarized it by adding up all the sales values for each sub-category. Right now it is showing data combined for all of our states, but let’s say we just want it to show one of them. We can **filter by state by dragging the State variable** (**Dimensions**, under **Location**) **over to the filters shelf** and selecting one state from the list – let’s **pick California** and **click OK**.

    ![The screen is pictured with the numbers 1 through 3, corresponding to the instructions above.]({{ '/assets/images/tableau_b2i_006.JPG' | relative_url }})

7. Now we have a bar graph showing the Sales by Sub-Category for California.

    ![The resulting bar graph after filtering.]({{ '/assets/images/tableau_b2i_007.JPG' | relative_url }})

8. Next let’s look at the **Marks** card. You should see 5 boxes labelled Colour, Size, Label, Detail, and Tooltip. You can use these to customize your visualization.

    ![Image highlighting the marks card.]({{ '/assets/images/tableau_b2i_008.JPG' | relative_url }})

9. **Click on colour**, and **change the colour** of the bars **to a different shade of blue**.

    ![Highlight of the Colour box in the Marks card with a drop-down menu emerging from it.]({{ '/assets/images/tableau_b2i_009.jpg' | relative_url }})

10. Click on **Size**, and **use the slider** to make the bars wider or narrower.

    ![Highlight of the Size box in the Marks card. A drop-down menu emerges from it with the slider button highlighted.]({{ '/assets/images/tableau_b2i_010.jpg' | relative_url }})

11. Click on **Label**. The Label section allows you to create and customize labels. We can click on show mark labels to see the values for each bar (under options, make sure to allow overlap as well), but you can see this makes our bar graph look cluttered, so let’s **keep the show mark labels unchecked**.

    ![Highlight of the Label box in the Marks card. A drop-down menu emerges from it with the 'Show mark labels' box highlighted.]({{ '/assets/images/tableau_b2i_011.jpg' | relative_url }})

12. Let’s add the broader category that the product falls under in the tool tip. To do this, **drag the Category variable** (**Dimensions,** under **Product**) to the tooltip box.

    ![Highlight of the Category variable in the Dimensions section as well as the Tooltip box in the Marks Card.]({{ '/assets/images/tableau_b2i_012a.jpg' | relative_url }})

    click on Tooltip. In the edit box, you will see “Category:” has been added underneath Sub-Category to the tooltip. However, if you want to change the order, perhaps to have the broader category go first, you can click on tooltip and edit the box. **Switch the order, making Category come before Sub-Category and click on OK.** 

    **![The screen is pictured with the numbers 1 and 2, corresponding to the instructions above.]({{ '/assets/images/tableau_b2i_012b.jpg' | relative_url }})**

13. You can also customize the axes. For example, **right click on your x-axis title, select edit axis**. Here you can make changes to your axis, such as the range of values or tick marks.

    ![Image displaying a menu emerging from the Sales axis. The menu item 'Edit Axis...' is selected.]({{ '/assets/images/tableau_b2i_013a.jpg' | relative_url }})

    **Change the title** (under **Axis Titles** in the **General** tab) to say “**Sales in US Dollars**”. Then close the window. The change will be applied automatically.

    ![Image displaying the Edit Axis window with the Title text box highlighted. "Sales in US Dollars" is in the text box.]({{ '/assets/images/tableau_b2i_013b.jpg' | relative_url }})

14. Right now the bars are sorted in alphabetical order by Sub-Category, but if you **hover over the x-axis label**, Sales in US Dollars, **a small sort icon appears**. **Click on it to sort your bars by sales** instead.

    ![Image highlighting the sort icon appearing beside the x-axis label.]({{ '/assets/images/tableau_b2i_014a.jpg' | relative_url }})

    Every time you click the icon, it cycles through different sort orders. Let’s have it sort descending with the sub-category with the largest sales at the top. You can now easily see the top and bottom sub-categories in terms of sales.

    ![Image displaying the resulting bar chart sorted descending by sales. ]({{ '/assets/images/tableau_b2i_014b.jpg' | relative_url }})

15. If we wanted to, we could also spread this visualization out a bit, so it is not squished up at the top. From the top ribbon **where it says Standard, use the drop-down to select Entire View**.

    ![Image highlighting the Fit Control drop down menu with the menu item "Entire View" highlighted.]({{ '/assets/images/tableau_b2i_015.jpg' | relative_url }})

16. Finally, we can give our visualization a more meaningful title by **double clicking where it says “Sales Bar” at the top**. You will see the default title is the sheet name, but we can change that. Let’s **put “Sales by Sub-Category for “** then instead of typing in “California”, we can make the title dynamic by **clicking on Insert and selecting State**. Then if we change the filter, the title will automatically change.

    ![The screen is pictured with the numbers 1 through 3, corresponding to the instructions above.]({{ '/assets/images/tableau_b2i_016.jpg' | relative_url }})

17. Let’s create one more bar graph, as we are going to use it later in the activities. Let’s create a similar bar graph but showing profit by sub-category. First, we need a new worksheet. **Click on the icon with “a plus sign in front of a bar graph”** to the right of “Sales Bar” at the bottom of the screen. That is the **new worksheet icon**.

    ![Image showing the New Worksheet icon.]({{ '/assets/images/tableau_b2i_017a.jpg' | relative_url }})

    Let’s **rename** this one to **“Profit Bar”.** 

    ![Image displaying the new added tab titled "Profit Bar".]({{ '/assets/images/tableau_b2i_017b.jpg' | relative_url }})

18. **Drag the Profit variable** (**Measures**) **next to columns and Sub-category** (**Dimensions**, under **Product**) **next to rows**.

19. Let’s colour the bars this time based on their profit (showing gains in shades of blue and losses in orange – a diverging colour palette). **Drag the Profit variable** (**Measures**) on to the **Colour** box in the **Marks** card.

    ![Highlight of the Profit variable in the Measures section as well as the colour box in the Marks Card.]({{ '/assets/images/tableau_b2i_019a.jpg' | relative_url }})

    In this case, the meaning of the colours is fairly clear, so we can hide the legend. **Hover over the legend until you see a small arrow**. **Click on it** to get the drop-down menu, and then **select Hide Card**.

    ![Image displaying a dropdown menu emerging from the legend with the menu item "Hide Card" highlighted.]({{ '/assets/images/tableau_b2i_019b.jpg' | relative_url }})

20. Finally, just **simplify the title** here by and put **“Profit by Sub-Category”** instead. You can see that this bar graph highlights the sub-categories that are making a loss or a large gain in profit quite clearly.

    ![Image displaying the final bar graph with the changed title "Profit by Sub-Category".]({{ '/assets/images/tableau_b2i_020.jpg' | relative_url }})

***
