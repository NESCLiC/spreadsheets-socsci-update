---
title: "Data type tips and tricks"
teaching: 15
exercises: 0
questions:
- "How can data types affect my ability to work with my data in a spreadsheet?"
objectives:
- "Recognize common spreadsheet data type issues and how to troubleshoot them."
- "Describe common solutions for data type issues."

keypoints:
- "Sometimes the issue with with the data type, not the data."
- "There are clues in your spreadsheet software that will alert you to possible issues."
- "You can get a sense of what might be happening by saving the data as a csv and looking at the text file."
---
## Data types

There are two main data types in most spreadsheet software - numbers and text. There are a variety of ways that the data can come to be in the cell (direct entry, drop-down lists, formulas, etc.) but those are the two most basic types of data you will come across. We will take a moment to look further into how spreadsheet software looks at each of these types.

### Numbers

Numbers are what spreadsheet software are best at, but this can cause problems if your data don't fit into built-in models and assumptions. If you open the Format Cells window you will notice that there is a tab called Number that allows you to pick a Category. The default category is usually General, which means there is no specific format. In the case of most numeric social science data you will probably most frequently use Number, but you might also use Date. Later in the workshop we will talk about some of the ways that date formatting can cause you problems. Use any of the types beside Number with caution, as they will change how the data appears but not how it exists if you export your file in a csv or format for statistical software. 

A visual cue that your data are being stored as numbers is that they will be right-justified. 

### Text

As is the case with numeric data, text will be stored with no formatting if the Category is General. Formatting the cells as text will mean that only functions that work on text will be allowed, so even if the data is numeric you won't be able to use arithmetic formulas. 

Text will be left-justified in the cell.

## Numbers stored as text

One of the advantages of storing data as text instead of numbers is that it will stay exactly as it is entered. This can be advantageous if you have numbers as a code for something else. 

A prime example of this are ZIP Codes; if you are working with ZIP Codes in the northeast US they have a leading '0'. For example, the ZIP Code for one part of Medford, MA, is 02155. When you have a column of ZIP Codes in a spreadsheet you might be tempted to format those cells as numbers, but if you do you will lose your leading zero and the ZIP Code will not be correct (2155 is not the same as 02155). 

If you have a column that you think should act as numbers but you get error messages, check to see if there are any warnings in your cells. In Excel, for example, if you have numbers stored as text there could be a small green flag in the top left corner of the cell and a warning message. If you can't change the cells to Number there might be a character in the column that can only be classified as text. Some possible causes of this are having a range of numbers (1-4, for example), typos, or text indicating missing values. You can prevent these kinds of issues using quality assurance, which we will talk about later in the lesson.

When you are deciding on which data type to use think about what the values in the column will be used for. If you will want to use math, you will need to designate your cells as **numbers**. If the values are codes you will not need to use mathematical formulas on them and you should designate them as **text**. If you find that you have a column that you want to designate as **General**, think about why. You might have mixed information in your column which may mean you want to rethink your columns.

## Formulas versus Values

When you use a formula in a spreadsheet the value is what appears in the cell, but the formula is what is actually stored there. This can cause issues when you want to export your dataset or use the column for more calculations. While you should always document the steps you took to get your final dataset, you can save a copy of your dataset that is just the values. 

You can use copy and paste to keep just the values. Copy your entire row of data and either create a new column or paste over the old column, but instead of using the normal paste you can Paste Special, and choose Values. 

Use this extremely carefully! If you have values that change that would have affected your calculated column these won't change. Only do this when you are done with any changes.

 






