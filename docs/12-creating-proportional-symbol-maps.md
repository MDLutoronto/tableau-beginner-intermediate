---
title: Creating Proportional Symbol Maps
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2020-03-25
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
nav_order: 12
---

## Creating Proportional Symbol Maps

1. Another type of map we can create using Tableau is a proportional symbol map, where the maps scales the size of simple symbols, like circles, proportionally to the data value found at that location. Let’s create a proportional symbol map showing GDP by country.

2. Again, we need a new worksheet. **Click on the new worksheet icon at the bottom of the screen. Let’s rename this one to “Proportional Map”.** 

3. Using the show me, as we have done before, **hold down the Ctrl key** and **select the Country/Region variable** (**Dimensions**) and **the GDP variable** (**Measures**, under **Development**), and then **click on Show Me**. **Select the proportional symbol option (the map with symbols).** 

    **![The Country/Region variable in the Dimensions section, the GDP variable in the Measures section and the Proportional Map option in the Show Me tab, all highlighted.]({{ '/assets/images/tableau_b2i_108.jpg' | relative_url }})**

4. Let’s change the legend to adjust the size of the symbols. **Hover over the legend until you see a small arrow. Click on it** to get the drop-down menu, and then **select Edit Sizes...** 

    ![The GDP legend dropdown menu with the "Edit sizes..." item highlighted.]({{ '/assets/images/tableau_b2i_109a.jpg' | relative_url }})

    **Use the slider** to make the symbols a bit larger, so they are more visible (to the end of the word smallest). Then **click on OK**.

    ![The Edit Sizes window with the "Mark size range" slider and the "OK" button highlighted.]({{ '/assets/images/tableau_b2i_109b.jpg' | relative_url }})

    From this map, we can see that there are a number of countries with a significant GDP in Europe.

    ![The final Proportional Symbol Map.]({{ '/assets/images/tableau_b2i_109c.jpg' | relative_url }})

5. There are many special design conventions to consider for map making. Check out the Data Visualization guide for cartography tips: [https://mdl.library.utoronto.ca/dataviz/specialty-visualization-areas](https://mdl.library.utoronto.ca/dataviz/specialty-visualization-areas)

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)