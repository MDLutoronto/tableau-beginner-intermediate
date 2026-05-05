---
title: Creating Dashboards
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
nav_order: 13
---

## Creating Dashboards

1. Now so far we have been creating visualizations within worksheets. But you can also create dashboards that combine a number of visualizations together to present a more complex story than a single visualization can show. **Click on the create new dashboard icon at the bottom, next to the new worksheet icon.** 

    **![Image showing the New Dashboard icon.]({{ '/assets/images/tableau_b2i_111.jpg' | relative_url }})**

2. You then can drag and drop various sheets to layout a dashboard. You can see it really helps to label your sheets. You can also drag other objects (bottom left), such as text or images to create your dashboard. So let’s create a dashboard showing sales and profit by sub-category and being able to filter by state.

    ![The Sheets and Objects sections in the Side Bar, both highlighted.]({{ '/assets/images/tableau_b2i_112.jpg' | relative_url }})

3. Before we start building our dashboard, I just want to adjust the Sales Bar sheet slightly. Go to the **Sales Bar sheet by clicking on its tab** at the bottom. **Right click on the State pill** on the **Filters** shelf, and **select Edit Filter...** 

4. **Select all and click on OK.** 

    ![The Filter window with the "All" and "OK" buttons highlighted.]({{ '/assets/images/tableau_b2i_114a.jpg' | relative_url }})

    Then **right click on the State pill** on the **Filters** shelf again, but this time **select Show Filter**.

    ![The drop-down menu for the State pill in the Filters Shelf. The drop-down menu item "Show Filter" is highlighted.]({{ '/assets/images/tableau_b2i_114b.jpg' | relative_url }})

    Now you can see the filters show up on the right. **Hover over the legend until you see a small arrow. Click on it** to get the drop-down menu, and then **select Single Value (dropdown)**.

    ![The legend drop-down menu with the item "Single Value (dropdown)" highlighted.]({{ '/assets/images/tableau_b2i_114c.jpg' | relative_url }})

    Now we have a State filter that the reader can use to filter the graph. We are going to take this filter and use it in our dashboard to apply to all the graphs we add into the dashboard.

5. So let’s go back to our dashboard by clicking on the **Dashboard 1** tab at the bottom.

6. First, let’s **drag the Sales Bar sheet into the dashboard**.

    ![The item Sales Bar in the Sheets section as well as the entire dashboard, both highlighted.]({{ '/assets/images/tableau_b2i_116a.jpg' | relative_url }})

    Then **drag the Profit Bar sheet underneath**.

    ![The item Profit Bar in the Sheets section as well as the bottom part of the dashboard, both highlighted.]({{ '/assets/images/tableau_b2i_116b.jpg' | relative_url }})

7. Our dashboard seems a bit squished, to improve how it displays, **under Size** on the left, **change Fixed size to Automatic.** 

    **![The Size drop-down menu with the sub-menu item "Automatic" highlighted. ]({{ '/assets/images/tableau_b2i_117.jpg' | relative_url }})**

8. To make the filter for the Sales sheet apply to both**, right click on the title of the filter, State, select Apply to Worksheets**, and then pick **Selected Worksheets...** 

    ![The State drop-down menu with the menu item "Apply to Worksheets" highlighted. The sub-menu item "Selected Worksheets..." is also highlighted.]({{ '/assets/images/tableau_b2i_118a.jpg' | relative_url }})

    **Click on All on dashboard**. Now you will see that when you select one state, both graphs refer to that state.

    ![The Apply Filter to Worksheets window with the "All on dashboard" and "OK" buttons both highlighted.]({{ '/assets/images/tableau_b2i_118b.jpg' | relative_url }})

9. Let’s add a title to our dashboard. **Drag Text from under objects to the top of the dashboard**. As you drag, make sure the grey rectangle is narrow, spanning the top of the whole dashboard.

    ![The Text item in the Objects sections as well as the top of the dashboard, both highlighted.]({{ '/assets/images/tableau_b2i_119a.jpg' | relative_url }})

    **Make the title “Sales and Profit by Sub-Category”, set the font size to 20 and make it bold**.

    ![The Edit Text window with the title "Sales and Profit by Sub-Category" entered.]({{ '/assets/images/tableau_b2i_119b.jpg' | relative_url }})

    **Resize the height of the title** to finish it off.

    ![The resulting dashboard with the resized Title.]({{ '/assets/images/tableau_b2i_119c.jpg' | relative_url }})

10. Finally, let’s add a dashboard action, where if you click on a sub-category in one of the graphs, it will highlight it in both to help the reader link the data together visually. From the **Dashboard menu** at the top, **select Actions...** 

    ![The Dashboard drop-down menu with the item "Actions..." highlighted.]({{ '/assets/images/tableau_b2i_120a.jpg' | relative_url }})

    **Click on the Add Action > and select Highlight...** 

    ![The Actions window with the "Add Action>" button highlighted. The "Add Action>" menu with the item "Highlight…" is also highlighted.]({{ '/assets/images/tableau_b2i_120b.jpg' | relative_url }})

    From this window, you could customize the settings if you wish to specify which sheets would be affected, and where to do it on hover or selection, for example. Let’s **keep the defaults and click on OK**. Then **click on OK again** to close the Actions window.

    ![The "Add Highlight Action" window with the "OK" button highlighted. ]({{ '/assets/images/tableau_b2i_120c.jpg' | relative_url }})

    Now if you select a Sub-Category in one graph, such as Chairs, it should highlight Chairs in the second graph. Click it again to deselect it.

    ![The resulting dashboard with highlighting capabilities displayed.]({{ '/assets/images/tableau_b2i_120d.jpg' | relative_url }})
