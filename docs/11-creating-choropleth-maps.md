---
title: Creating Choropleth Maps
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
nav_order: 11
---

## Creating Choropleth Maps

1. Another type of visualizations we can create with Tableau is maps. Let’s create a couple now to show spatial patterns. First, we will create a choropleth map, where areas are proportionally colour-coded to represent a variable. Let’s create a choropleth map showing infant mortality by country.

2. Again, we need a new worksheet. **Click on the new worksheet icon at the bottom of the screen. Let’s rename this one to “Choropleth Map”.** 

3. Using the show me, as we have done before, **hold down the Ctrl key** and **select the Country/Region variable** (**Dimensions**) and **the Infant Mortality Rate variable** (**Measures**, under **Health**), and then **click on Show Me**. **Select the maps option with shaded areas.** 

    **![The Country/Region variable in the Dimensions section, the Infant Mortality Rate variable in the Measures section and the Choropleth Map option in the Show Me tab, all highlighted.]({{ '/assets/images/tableau_b2i_104.jpg' | relative_url }})**

4. Let’s change the legend from an unclassed map to a simplified classed map, having five different shades of blue corresponding to bin or ranges of values for infant mortality rate. **Hover over the** legend until you see a small arrow. Click on it to get the drop-down menu, and then **select Edit Colours...** 

    ![The Infant Mortality legend drop-down menu with the item "Edit Colours..." highlighted.]({{ '/assets/images/tableau_b2i_105a.jpg' | relative_url }})

    **Click on Stepped Colour** and keep the default of five colours. Then **click on OK**.

    ![The Edit Colours window with the option "Stepped Colour" checked and highlighted.]({{ '/assets/images/tableau_b2i_105b.jpg' | relative_url }})

    From this map, we can see that infant mortality is higher in Africa and parts of Asia compared to the rest of the world.

    ![The final Choropleth Map.]({{ '/assets/images/tableau_b2i_105c.jpg' | relative_url }})
