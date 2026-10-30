**Date**<br>
**MPAD 2003 Data Storytelling**<br>
**Luwi Kabaso**<br>
**Presented to Jean-Sébastien Marier**<br>

# Deliverable 2: Exploratory Data Analysis (EDA)

Use one hashtag symbol (`#`) to create a level 1 heading like this one.

## Foreword

For this assignment, you must clean and analyze the dataset from Deliverable 1, create exploratory charts/visualizations, and identify a potential story. Your assignment must clearly detail your process. You are expected to write about 1,000-1,200 words, and to include several screen captures showing the different steps you went through. Your assignment must be written with the Markdown format and submitted on GitHub.

I have been assigning different versions of this project to my digital journalism and data storytelling students for a few years now. Its structure was inspired by the main sections/chapters of [*The Data Journalism Handbook*](https://datajournalism.com/read/handbook/one/). This version was further inspired by the [Key Capabilities in Data Science](https://extendedlearning.ubc.ca/programs/key-capabilities-data-science) program offered by the University of British Columbia (UBC).

**Here are some useful resources for this assignment:**

* [GitHub's *Basic writing and formatting syntax* page](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* [The template repository for this assignment in case you delete something by mistake](https://github.com/jsmarier/jou4100_jou4500_mpad2003_project2_template)

Did you notice how to create a hyperlink? In Markdown, we put the clickable text between square brackets and the actual URL between parentheses.

And to create an unordered list, we simply put a star (`*`) before each item.

## 1. Getting Data

Use two hashtag symbols (`##`) to create a level 2 heading like this one.

To include a screen capture, use the sample code below. Your images should be saved in the same folder as your `.md` file.

![](import-screen-capture.png)<br>
*Figure 1: The "Import file" prompt on Google Sheets.*

**Here are examples of functions and lines of code put in grey boxes:**

1. If you name a function, put it between "angled" quotation marks like this: `IMPORTHTML`.
1. If you want to include the entire line of code, do the same thing, albeit with your entire code: `=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)`.
1. Alternatively, you can put your code in an independent box using the template below:

``` r
=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)
```
This also shows how to create an ordered list. Simply put `1.` before each item..

For this assignemnt I will be analyzing the dataset on traffic colliosns from open ottawa to see what role road and weather conditions played in the cause of the collision and if any pattern can be derived from this. Originally I planned on using `IMPORTDATA` to extract the data from the dataset however I would soon find out that would be impossible to do on open ottawa so I resorted to doing it manually by downloading the csv and importing it from file. (https://docs.google.com/spreadsheets/d/1PMjr_dMFUb8QtXqLGrBA_43ulSd87OVDIKUuzPKIOYg/edit?usp=sharing) 

![](SS.png)<br>
*Figure 1: The imported data.*


Once i did that I selected the rows with the data I needed only as there were originally 17 columns but I only needed atleast 8 such as column N which had ordinal vairables on the conditions of the road, column R which had quantitive ratio variables on the number of cars involved and column L also with ordinal variables. but covering the classification of the accidents. There were also over a thousand rows as the data ranged from the years 2017 to 2024 (excluding 2023) so I decided to create seperate sheets for each of the years, i.e 2017 - 2018,  2019 - 2020 and so on. (https://docs.google.com/spreadsheets/d/1a3oO_SJUtO0-cOCRndJqsE5OG9lnO--kZDpro2BcLkY/edit?usp=sharing)

![](SS2.png)<br>
*Figure 1: The data imported into seperate sheets*

I created these sheets in a seperate file and planned on using `IMPORTRANGE` to put get the desired columns and rows in there. However before I could do that I had to make sure the rows were ordered correctly else it would be a mess upon importation. After reviewing it all I saw that some of the years were mixed together and were not properly in accending order so by using the advanced range sorting options I ordered it correctly. I also used the data cleanup tool to get rid of white spaces as well. After all that I imported the data as planned



## 2. Understanding Data

### 2.1. VIMO Analysis

Use three hashtag symbols (`###`) to create a level 3 heading like this one. Please follow this template when it comes to level 1 and level 2 headings. However, you can use level 3 headings as you see fit.

Insert text here.

Support your claims by citing relevant sources. Please follow [APA guidelines for in-text citations](https://apastyle.apa.org/style-grammar-guidelines/citations).

**For example:**

As seen in Bounegru & Gray (2011), a data visualization should be clear...

### 2.2. Cleaning Data

Insert text here.

### 2.3. Analyzing Data

Insert text here.

**This section should include a screen capture of your pivot table, like so:**

![](pivot-table-screen-capture.png)<br>
*Figure 2: This pivot table shows...*

**This section should also include a screen capture of your exploratory chart, like so:**

![](chart-screen-capture.png)<br>
*Figure 3: This exploratory chart shows...*

## 3. Delivering Data

Insert text here.

## 4. References

Include a list of your references here. Please follow [APA](https://apastyle.apa.org/style-grammar-guidelines/references) or [MLA](https://www.mla.org/MLA-Style) guidelines for references. Hanging paragraphs aren't required though.

**Here's an example:**

Bounegru, L., & Gray, J. (Eds.). (2021). *The Data Journalism Handbook 2: Towards A Critical Data Practice*. Amsterdam University Press. [https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153](https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153)
