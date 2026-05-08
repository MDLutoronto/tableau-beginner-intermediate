---
title: Creating Scatter Plots
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2020-03-25
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
nav_order: 7
---


## Creating Scatter Plots

1. Sometimes you have to pull data from multiple sources instead of having it all in one file. Let’s add a couple more datasets, but this time we’re going to match them up or join them together to create one large dataset to work from.

2. Go to the top **Data** Menu and select **New Data Source**. Select **Microsoft Excel** and **choose the *AuthorDataCitationsGrants.xls*** file. This is the dataset that contains the names of authors, their institutions and countries, and amount of citations and grant money they have received over a few years.

    ![Tableau's connect menu with the menu-item "Microsoft Excel" highlighted.]({{ '/assets/images/tableau_b2i_067.jpg' | relative_url }})

3. Now **click on Add** next to **Connections** on the top left to add a second dataset. Select **Microsoft Excel** and then **pick the *AuthorDataExperience.xls*** file. This dataset has just author names, along with how many years of experience they have as a researcher.

    ![The "Add" button as well as the item "Microsoft Excel" in the "Add a Connector" window both highlighted.]({{ '/assets/images/tableau_b2i_068.jpg' | relative_url }})

4. To relate or connect the two datasets, **drag** **AuthorDataExperience** under Sheets over to the section where it says, “Need more data?” (if you don't see  AuthorDataExperience under Sheets, make sure that AuthorDataExperience is selected under Connections).  

    <img src='{{ '/assets/images/TableauIntermediateUpdate-69.jpg' | relative_url }}' alt='' title='' width='1909' height='953' />

    The pop up window shows us that the data has been related together based on a common column, Author. Now the years of experience data will also be associated with the appropriate authors additional data found in the first table. Tableau performs relates and joins on the fly, as needed. If these terms are new to you, see [this article on relationships and joins in Tableau](https://help.tableau.com/v2020.2/pro/desktop/en-us/datasource_relationships_learnmorepage.htm) for more info). Click on the “x” to **close the pop up window**. 

    ![The Edit Relationship window with the close button highlighted.]({{ '/assets/images/tableau_b2i_069b.jpg' | relative_url }})

5. Next, we can **click on a new worksheet icon at the bottom. Let’s rename this one to “Scatter Plot”.** 

6. Scatter Plots are great to use to identify if there is any relationship between numeric variables. Let’s see if there is a correlation between grants and years of experience.

7. Again, let’s create this scatterplot using the Show Me feature. This time, **hold down the Ctrl key** and **select the Grants variable** (**Measures**, under **AuthorDataMain**) and the **Years of Experience****variable** (**Measures**, under **AuthorDataExperience**), and then **click on Show Me** to expand the tab. **Select the scatter plots**, one of the recommendations.

    ![Highlight of the Grants and Years of Experience variable in the Measures section as well as the Scatter Plot item in the "Show Me" tab all highlighted.]({{ '/assets/images/tableau_b2i_072.jpg' | relative_url }})

8. Does not look like much yet, but let’s make some adjustments. First, instead of summing these variables, let’s take the averages. So **right click on the Grants pill, select Measures (Sum)** and then **change it to Average**. **Do the same for the Years of Experience pill**.

    ![Dropdown menu from the "Grants" pill with the "Measure(Sum)" item selected. From this item the sub-menu item "Average" is highlighted.]({{ '/assets/images/tableau_b2i_073.jpg' | relative_url }})

9. Our next problem is that it is plotting just one x/y pair – the averages of the whole dataset. We need to plot the points for each author, country, or institution. Let’s do it by author. This is where that details box comes up. If you **drag the Author variable** (**Dimensions**, under **AuthorDataMain**) over to the **Details** box on the **Marks** card, it explodes out the aggregation to plot it by author. When you hover over a point, you can see the details.

    ![Author variable in the Dimensions section as well as the Detail box in the Marks card are highlighted.]({{ '/assets/images/tableau_b2i_074.jpg' | relative_url }})

10. You may notice there is now also another box on the Marks card called Shapes. If you want to add another categorical variable to your scatterplot, you could do so by using different shape to represent different categories. **Drag the Institution variable** (**Dimensions,** under **AuthorDataMain**) on to the **Shapes** box on the **Marks** card. Now you should see that there is a legend on the right, using different shapes for different institutions.

    <img src='{{ '/assets/images/TableauIntermediateUpdate-75.jpg' | relative_url }}' alt='' title='' width='1643' height='1001' />

11. If you want to add trend lines in Tableau, right click in the centre of the graph and **select Trend** Lines, and then select **Show Trend Lines**. Hovering over the lines also gives you statistical information, such as p-values.

    ![The Scatter Plot settings menu window with the item "Trend Lines" highlighted. From this menu item, the sub-menu item "Show Trend Lines" is also highlighted.]({{ '/assets/images/tableau_b2i_076.jpg' | relative_url }})

12. Finally, one interesting feature of Tableau is to create not just one visualization, but a series of them, using the Pages shelf. **Drag the Year variable** (**Dimensions,** under **AuthorDataMain**) on to the **Pages** shelf. Now you should see some controls on the right. The user can scroll through three different scatterplots, one for each year, or they can click on the play button to have it animate through the years.

    <img src='{{ '/assets/images/TableauIntermediateUpdate-77.jpg' | relative_url }}' alt='' title='' width='1648' height='881' />

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)