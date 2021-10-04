<p><img src="https://www.rug.nl/about-ug/practical-matters/huisstijl/logobank-new/corporatelogo/corporatelogorood/rugr_logonl_rood_rgb.png" width="200" alt="rug logo"></p>

# Analyzing Data - A Practical Guide
<img src="https://img.shields.io/badge/academic%20year-2021--2022-red">
<p>By <a href="https://www.linkedin.com/in/jmperafan/">Juan Manuel Perafan</a></>

---
## **Exercises**

This document contains every exercise we will be conducting during the lectures. 

---
<details>
  <summary>Lecture 1</summary>

  ### **1.0 Introduction**
  Introduce yourself:
  - Name.
  - Study.
  - What do you expect from this course?

  <br></br>
  
  ### **1.1 Go Full Stalker**
  Imagine your objective is to create a digital trail of somebody's day. Make it at detailed as possible. Your exercise now is to think:

  - What type of data could you collect?
  - What practical problems would you run into? 
  
  <br></br>

  ### **1.2 Create KPI's**
  Choose any organization and imagine you work for them. Your objective is to:

  - Think about possible KPI's (i.e. key performance indicator).
  - Speculate how they can be measured.

  <br></br>

  ### **1.3 The Rat Factory**
  
  ```
  In 1902, in Vietnam, the colonial government created a bounty program that paid a reward for each rat killed. Vietnamese rat catchers quickly realized breeding rats was easier and profitable than catching them. 
  ```

  What you just read is an example of a perverse incentive (also known as cobra effect). Using your input for the previous exercise, your task is:

  - Think how an employee could exploit these KPI's.
  - Explore scenarios where it can be counter-productive.
  
</details>


<details>
  <summary>Lecture 2</summary>
  
  ---
  
  ### **2.0 Spreadsheet Galore**
  Imagine your organization wants to store operational data in a spreadsheet (e.g. Excel). 

  1. Do you think this is a good idea or not? 
  2. What can go wrong?
  3. Can you mitigate some of these issues by using the cloud version (e.g. Google Sheets)?

  <br></br>

  ### **2.1 Types Flat Files**

  1. Google the differences between a `csv file`, a `JSON file`, and a `parquet file`. Research them enough to understand when it is a good idea to use one over the other.

  2. Copy the text below into `Notepad` (or any text editor) and save it as `cars.csv`

  ```
  Year,Make,Model
  1997,Ford,E350
  2000,Mercury,Cougar
  ```
  3. Transform the text into a `JSON file` and save it as a new file called `cars.json`. Make sure you keep both files. It is also up to you if you want to transform them manually or use a website.

  4. Try to open both in Tableau. Do you notice any differences?

  <br></br>

  ### **2.2 Connect to a database**

  1. Open Tableau and connect to `Microsoft SQL Server`. Once the prompt opens, put in the following credentials:

  - Server: `3.143.125.139`
  - Authentication: `Use a specific username and password`
  - Username: `SQL`
  - Password: `SQL`

  Leave everything else empty and unchecked. 

  2. Explore the different databases and tables inside. Try to guess what each database is used for. For example, which ones are automatically generated.

  <br></br>

  ### **2.3 Working with APIs**

  1. Go to any browser and go to this site `https://openlibrary.org/search/authors.json?q=j%20k%20rowling`

  2. Replace `j%20k%20rowling` by the name of any other author. 

  Note: As you might have infered, `%20` is [HTML URL Encoding](https://www.w3schools.com/tags/ref_urlencode.ASP) for a space. There is at least one encoding for every character, but `%20` is the most common, since URLs cannot have spaces. Also, if `%20` feels a bit difficult to remember, you can also use `+`.

  <br></br>

  ### **2.4 Web Data Connector**

  1. Go to https://www.makeovermonday.co.uk/data/

  2. Pick any dataset.

  3. Open the link under the data column.

  4. You will be redirected to [data.world](data.world). You can find all sorts of public datasets in here. Most of them are perfect for your final project.

  5. Either create an account (you might be using this site more in the future) or use the following credentials to sign in:

  - Username: hc-analyzing-data
  - Password: analyzing-data

  5. Look for the `Open in app` button. The one with the three empty squares and the diamond at the top right of the dataset.

  <img src="https://media.data.world/KVWgC7jTjWaDkId1ub4Y_Screen%20Shot%202018-04-20%20at%202.14.07%20PM.png" />

  6. Follow the instructions and open it as a Web Data Connector in Tableau.

</details>

<details>
  <summary>Lecture 3</summary>

  ---
  
  ### **3.0 What is wrong with this data?**
  Your objective is to create a file with how this data is supposed to look once it is clean. It is ok if you don't know the name of the steps. For now, just think of how the clean dataset will look like.

<table class="table table-bordered table-hover table-condensed" style="border:1px solid black;margin-left:auto;margin-right:auto;">
   <thead>
      <tr>
         <th title="Field #1">name</th>
         <th title="Field #2">job</th>
         <th title="Field #3">age</th>
         <th title="Field #4">salary 2020</th>
         <th title="Field #5">salary 2021</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>john</td>
         <td> </td>
         <td> 21 years</td>
         <td align="right"> 0</td>
         <td align="right"> 1000</td>
      </tr>
      <tr>
         <td>JANE JOHNSON</td>
         <td> analyst</td>
         <td> 24</td>
         <td align="right"> $3500</td>
         <td align="right"> $4000</td>
      </tr>
      <tr>
         <td>Charlie</td>
         <td> chef</td>
         <td> fourty</td>
         <td align="right"> 30000</td>
         <td align="right"> 32000</td>
      </tr>
   </tbody>
</table>
  
  <br></br>
  
  ### **3.1 Cleaning a real-world data**

  You are going to be exploring and cleaning a real-world dataset here. All of the data comes from a real survey with thousands of participants.

  1. Check the [survey](https://www.askamanager.org/2021/04/how-much-money-do-you-make-4.html) and spot questions that might lead to data quality issues.

  2. Check the [answers](https://docs.google.com/spreadsheets/d/1IPS5dBSGtwYVbjsfbaMCYIWnOuRmJcbequohNxCyGVw/edit?resourcekey#gid=1625408792). Were you assumptions about the last question correct?

  3. Think what type of cleaning is needed to answer the following question: What is the average salary per race?

  4. Think of which rows you should filter. What to do with empty rows, with people outside of the US, people with no salary, duplicates or partial duplicates, and salaries that seem either too high or too low. This is not a science, it is a matter of judgement.

  5. Try to standarize the salary. Think of what to do with the column containing `Other monetary comp` and how you can turn other currencies into dollars (or whatever other currency you prefer).

  6. Look at the `Country` column. How are you going to standarize it? Here is a rule of thumb, if you are cleaning:

  - < 10 values: Use [logical formulas](https://help.tableau.com/current/pro/desktop/en-us/functions_functions_logical.htm)  like `IF` and `CASE` or [use Groups in Tableau](https://www.guru99.com/tableau-sort-data.html). It is a manual option, but it is much better for performance.

  - 10+ values: Create a new table (or spreadsheet) with 2 columns. One containing all of the unique values currently in the dataset and a second column with the clean value (your table should look like the one below). Once you are done, join both tables and only keep the correct one.

<table class="table table-bordered table-hover table-condensed" style="border:1px solid black;margin-left:auto;margin-right:auto;">
   <thead>
      <tr>
         <th title="Field #1">Raw</th>
         <th title="Field #2">Clean</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>US</td>
         <td> United States</td>
      </tr>
      <tr>
         <td>USA</td>
         <td> United States</td>
      </tr>
      <tr>
         <td>U.S.A.</td>
         <td> United States</td>
      </tr>
      <tr>
         <td>United States</td>
         <td> United States</td>
      </tr>
      <tr>
         <td>America</td>
         <td> United States</td>
      </tr>
   </tbody>
</table>
  
  <br></br>

  ### **3.2 The Next Birthday?**
  Your company wants a dashboard that shows how many days until the next birthdays or anniversaries. The data looks something like this:

  ```
  employee_id, birthday, anniversary
  1, 10 April, 15 October
  2, 1 January, 1 December
  3, 7 September, 1 November
  4, 22 July, 1 July
  ```

  1. Copy and paste this dataset into Tableau. [Here is a tutorial on how to do it](https://www.thedataschool.co.uk/jonathan-allenby/tableau-tip-you-can-paste-data-directly-into-tableau). Make sure the data is imported correctly (commas as separators).

  2. Find a way to clean the dates. You were provided a day and a month, but the year is missing. If you just [change the data type to date](https://help.tableau.com/current/pro/desktop/en-us/datafields_typesandroles_datatypes.htm), Tableau will infer the year 1900.

  3. You don't need to do this, but there are some advantages in [pivoting](https://help.tableau.com/current/pro/desktop/en-us/pivot.htm) both of the date columns (i.e. anniversary and birthday). Why don't you try creating a dataset that looks like this:

  <table class="table-bordered table-hover table-condensed" style="border:1px solid black;margin-left:auto;margin-right:auto;">
    <thead>
        <tr>
          <th title="Field #1">employee_id</th>
          <th title="Field #2">event_type</th>
          <th title="Field #3">date</th>
        </tr>
    </thead>
    <tbody>
        <tr>
          <td align="right">1</td>
          <td> birthday</td>
          <td> 10 April</td>
        </tr>
        <tr>
          <td align="right">1</td>
          <td>  anniversary</td>
          <td> 15 October</td>
        </tr>
        <tr>
          <td align="right">2</td>
          <td> birthday</td>
          <td> 1 January</td>
        </tr>
        <tr>
          <td align="right">2</td>
          <td>  anniversary</td>
          <td> 1 December</td>
        </tr>
    </tbody>
  </table>

  4. Try to calculate when will be the next birthday or anniversary. A big part of the job of an analyst is to Google these types of things, so I would advise you to do that instead of peaking at the hints. 

  <details>
    <summary>Here is a hint.</summary>
    If the date hasn't happened yet this year, then the right year is `YEAR(TODAY())`. If the date happened already, the right year is `YEAR(TODAY()) + 1`. 

    The result that you requires the following ingredients: `MAKEDATE()`, `YEAR()`, `TODAY()`, `IIF()`.

    In case you are wondering, `IIF()` is short for Intermediate IF. While in a normal `IF` statement you can add as many conditions as you want, `IIF()` only accepts one clause. In plain English, if something then this, otherwise that. 
  </details>

  <details>
    <summary>Fine, here is the answer.</summary>

  You need two formulas, one that calculates the date this year. It will look something like this:

  ```
  MAKEDATE( 
    YEAR(TODAY()), 
    MONTH([Date]),
    DAY([Date])
  )
  ```

  The second formula is the date next year. 

  ```
  MAKEDATE( 
    YEAR(TODAY()) + 1, 
    MONTH([Date]),
    DAY([Date])
  )
  ```

  The final formula compares if the date has already happened. 

  For this one, I assume you called the first formulas `Date This Year` and then second formula `Date Next Year`. This won't work if you gave the formulas a different name.

  ```
  IIF(
    [Date This Year] > TODAY(),
    [Date This Year],
    [Date Next Year]
  )
  ```
  </details>

  <pr></pr>

  5. Now use `TODAY()` and the formula you calculated in step 4 and find out how many days left before the next important dates.

  <details>
    <summary> Fine, here is the answer </summary>
    
    ```
    DATEDIFF(
      'day',
      [Date Next Year],
      TODAY()
    )
    ```
  </details>
  
  <pr></pr>

  6. Filter to include only the top 5 events. [Check TOPN filters](https://playfairdata.com/how-to-use-index-for-easier-top-n-tableau-filters/).

</details>