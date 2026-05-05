---
title: Creating Histograms
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
nav_order: 5
---

## Creating Histograms

1. Let’s try a different dataset for the next couple visualizations. We are going to load in external data this time. Go to the top **Data menu** and **select New Data Source**.

    ![Data dropdown menu with the menu item "New Data Source" highlighted.]({{ '/assets/images/tableau_b2i_050a.jpg' | relative_url }})

    Choose **Text,** and **select *iris.csv*** and **click Open**.

    ![Tableau's connect menu with the menu-item "Text file" highlighted.]({{ '/assets/images/tableau_b2i_050b.jpg' | relative_url }})

2. From this screen, you get a preview of the data. This dataset contains measurements for different parts of different species of iris flowers.

    ![The Data Source Page Display page. The data table for the loaded dataset is displayed.]({{ '/assets/images/tableau_b2i_051.jpg' | relative_url }})

3. The next visualization we are going to make is a histogram, which can show us the distribution of a numeric variable – for example, we could look at the frequency that different petal widths were recorded for different specimens of irises.

4. Again, we need a new worksheet. **Click on the new worksheet icon at the bottom of the screen. Let’s rename this one to “Histogram”.** 

5. This time, let’s take a look at creating the histogram demonstrating the show me feature. **Select the Petal.Width variable** (**Measures**), and then **expand Show Me by clicking on it**. You will see that there are two options that are not greyed out – a bar graph and a histogram. You can hover over any of the images in the Show Me tab to see what the visualization is called; it will be listed below. **Select the histogram**. Then **click on Show Me again** to close the tab.

    ![The Petal.Width variable in the Measures section along with the Histogram image in the Show Me tab both highlighted.]({{ '/assets/images/tableau_b2i_054.jpg' | relative_url }})

6. Let’ s colour by species – **drag the Species variable** (**Dimensions**) to the **Colour** box on the **Marks** card. You can see that depending on the species, there is a different range of petal widths.

    ![Image displaying the histogram, coloured by species.]({{ '/assets/images/tableau_b2i_055.jpg' | relative_url }})

7. Let’s filter by species so we can see the histogram for each species individually. **Drag the Species variable** (**Dimensions**) on to the **Filters** shelf and **make sure only Virginica is selected**, and then **click OK**.

    ![The Filter window with the item "virginica" and the "OK" button highlighted.]({{ '/assets/images/tableau_b2i_056a.jpg' | relative_url }})

    You can see that for Virginica, most of the flower’s petal widths are in the middle of the range of options.

    ![Image displaying the resulting histogram for the Virginica species.]({{ '/assets/images/tableau_b2i_056b.jpg' | relative_url }})

8. You may have also noticed that Tableau automatically creates a bin size variable under Dimensions to create the graph, where bins are just used to divide the Petal.Width variable into equal parts or ranges that each observation could fall under and their frequency could be calculated. Tableau automatically tries to select an appropriate bin size, but if you wanted, you could right click on Petal.Width (bin) under Dimensions and change the size of the bins. Let’s leave it as is for now.