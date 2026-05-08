---
title: Creating Box Plots
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2020-03-25
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
nav_order: 6
---

## Creating Box Plots

1. Related to a histogram is a box plot, so let’s create one now. Box plots show distribution in quartiles, and have a very compact display so you can compare distributions of multiple groups much easier than you could with side by side histograms. So instead of using colours on our histogram, as we did before we filtered it, let’s create a box plot to compare the distributions of petal width by species.

2. Again, we need a new worksheet. **Click on the new worksheet icon at the bottom of the screen. Let’s rename this one to “Box Plot”.** 

3. Let’s use the Show Me option again. This time **hold down the Ctrl key** and **select the Petal.Width variable** (**Measures**) and the **Species variable** (**Dimensions**), and then **click on Show Me** to expand the tab. **Select the box-and-whisker plots option**. Then **click on Show Me again** to close the tab.

    ![Highlight of Pedal.Width and Species variables in the Measures and Dimensions sections respectively as well as the Box-Plot option in the Show Me tab.]({{ '/assets/images/tableau_b2i_060.jpg' | relative_url }})

4. We change some of the settings on the box plot by **right clicking on it and selecting Edit...** 

    **![Box-Plot settings menu with the item "Edit..." highlighted.]({{ '/assets/images/tableau_b2i_061.jpg' | relative_url }})**

5. You can change what the whiskers (those line thin lines extending out from the box) represent. **From the drop-down, select Maximum extent of the data.** We can also **select Hide underlying marks (except outliers)** to remove the dots shown underneath the box and whiskers. Then **click on OK**.

    ![Edit window with both the item "Maximum extent of the data" in the drop-down menu and the "Hide underlying markers (excerpt outliers)" check box highlighted.]({{ '/assets/images/tableau_b2i_062.jpg' | relative_url }})

6. The box plot uses the whiskers to show us the high and low values (and the range of values for Petal width), and the median petal width (which is the middle line in the box). It also shows you that 50% of values in the dataset fall within the box.

7. But I mentioned the power of box plots is that you can compare different distributions. So let’s compare distributions of petal width by species. So **drag Species** (**Dimensions**) **next to columns**. You will see that you have split the data into three species, but the boxes are gone because currently it is aggregating the data to the sum for each species. To fix this, go to the **Analysis menu** at the top and **deselect Aggregate Measures**.

    ![The Analysis menu with the item "Aggregate Measures" highlighted.]({{ '/assets/images/tableau_b2i_064.jpg' | relative_url }})

8. Finally, you can hover near the species labels at the bottom to get an arrow cursor so you can click and **expand the graph’s width to be able to read the species labels**.

    ![Highlight of the species label at the bottom of the box plot graph.]({{ '/assets/images/tableau_b2i_065a.jpg' | relative_url }})

    You can see this graph shows us for example that the species Virginica has a largest range of petal widths and that there are some overlap in petal widths between Versicolor and Virginica, but none with Setosa.

    ![The final box plot.]({{ '/assets/images/tableau_b2i_065b.jpg' | relative_url }})

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)