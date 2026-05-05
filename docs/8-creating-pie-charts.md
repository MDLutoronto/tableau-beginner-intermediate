---
title: Creating Pie Charts
parent: Getting Started with Tableau Desktop (Beginner to Intermediate)
layout: default
nav_order: 8
---

## Creating Pie Charts

1. Okay let’s try a new dataset – this time some qualitative humanities data. Tableau is not meant to work directly with text data files, but you can use other better-suited textual analysis tools to create datasets that you can then visualize in Tableau. I downloaded the freely available full text of Shakespeare’s Romeo and Juliet. I separated it out into one text file per act. Then I uploaded all of the files to an online tool called Voyant Tools: [https://voyant-tools.org/](https://voyant-tools.org/). It calculated word frequencies for each act, which I now have in a spreadsheet. When Voyant calculated word frequencies, it also removed common words like “the” or “a”. These words are called stop words. If you want to learn more about textual visualization tools, such as Voyant, you can take a look at the Tools & Tutorials page in the guide: [https://mdl.library.utoronto.ca/dataviz/tools-tutorials](https://mdl.library.utoronto.ca/dataviz/tools-tutorials).

2. Let’s load this word frequency data into Tableau. Again, go to the top **Data** Menu and select **New Data Source**. **Select Microsoft Excel** and **pick *RomeoAndJulietWordFrequenciesByAct.xls***.

3. You can see that it is a simple spreadsheet that counts how many times a term/word came up in each act. Let’s **click on new worksheet to get started. Let’s rename this one to “Pie”.** 

4. Let’s first make a simple pie chart to show how many words are in each Act of the play, to see which Act is the longest and shortest and how they contribute to the whole.

5. Before we begin building our visualization, let’s make sure our variables are correct. If we look at what the variable types Tableau’s has identified in our dataset, you will notice that it thinks Act is a numeric variable in the measures section, when really it is categorical in this case. So let’s change it to move it to our dimensions section. **Drag the Act variable (Measures) into the Dimensions section (above "Term" in the variables list)**.

    ![The Act variable in the Measures section highlighted and an arrow beside it pointing towards to Dimensions section.]({{ '/assets/images/tableau_b2i_082.jpg' | relative_url }})

6. Using the Show Me feature, as we have done before, **hold down the Ctrl key** and **select the Act variable** (**Dimensions**) and the **Count variable** (**Measures**), and then click on Show Me to expand the tab. **Select the pie charts**, one of the recommendations.

    ![The Act and Count variables in the Dimensions and Measures sections as well as the pie chart option in the Show Me tab all highlighted. ]({{ '/assets/images/tableau_b2i_083.jpg' | relative_url }})

7. It is very small, so let’s make it larger. From the top ribbon **where it says Standard, use the drop-down to select Entire View**.

    ![The Fit Control drop-down menu with the menu item "Entire View" highlighted.]({{ '/assets/images/tableau_b2i_084.jpg' | relative_url }})

8. Next, let’s label it. **Drag the Act variable** (**Dimensions**) on to the **Label** box on the **Marks** card, and then **drag the Count variable** (**Measures**) on to **Label** box as well. Then **click on the Label box**, and **click on the ... icon next to the Text field** to edit the label. **Add the word “Act” to just before the act number** to clarify the label, and then **click on OK**. Then **click away to close the window**.

    ![The screen is pictured with the numbers 1 through 3, corresponding to the instructions above.]({{ '/assets/images/tableau_b2i_085.jpg' | relative_url }})

9. Current it is showing the frequency count as a raw number, but we could show a percentage of the total instead, which is more common for pie charts. **Right click on the SUM (Count) label pill** (the last one listed on the Marks card). **Select Quick Table Calculation** and then **Percent of Total**.

    ![The Sum(Count) label pill menu with the item "Quick Table Calculation" highlighted. From this item, a sub-menu item "Percentage of Total" is highlighted. ]({{ '/assets/images/tableau_b2i_086.jpg' | relative_url }})

10. We could also format the percentages to round to whole numbers. **Right click on the SUM (Count) label pill** again and this time **select Format**. From the format window that appears on the left, in the pane tab, under the default section, from the **drop-down for Numbers**, **select Percentage** and then **change the number of decimals to zero**. Then **click away** to close the window.

    ![The Format Pane with the Number drop-down menu. In this drop-down menu, the item "Percentage” is highlighted as well as the "Decimal places" input box.]({{ '/assets/images/tableau_b2i_087.jpg' | relative_url }})

11. We can see the number of words used is quite evenly distributed throughout the acts, but Act 3 uses the most and Act 5 uses the least.
