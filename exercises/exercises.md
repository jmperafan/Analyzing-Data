<p><img src="https://www.rug.nl/about-ug/practical-matters/huisstijl/logobank-new/corporatelogo/corporatelogorood/rugr_logonl_rood_rgb.png" width="200" alt="rug logo"></p>

# Analyzing Data - A Practical Guide
<img src="https://img.shields.io/badge/academic%20year-2021--2022-red">
<p>By <a href="https://www.linkedin.com/in/jmperafan/">Juan Manuel Perafan</a></>

---

## **Exercises**

This document contains every exercise we will be conducting during the lectures. 

---

<details>
  <summary><h2>Lecture 1</h2></summary>

### **1.0 Introduction**
Introduce yourself:
- Name
- Study
- What do you expect from this course?

### **1.1 Go Full Stalker**
Imagine your objective is to create a digital trail of somebody's day. Make it at detailed as possible. Your exercise now is to think:

- What type of data could you collect?
- What problems would you run into?Go Full Stalker

### **1.2 Create KPI's**
Choose any organization and imagine you work as a dataprofessional for them. Your objective is to:

- Think about possible KPI's.
- Speculate how they can be measured.

### **1.3 The Rat Factory**
Using your input for the previous exercise, your task is:

- Think how an employee could exploit these KPI's.
- Explore scenarios where it can be counter-productive.

</details>

<details>
  <summary><h2>Lecture 2</h2></summary>

### **2.0 Spreadsheet Galore**
Imagine your organization wants to store operational data in a spreadsheet (e.g. Excel). Do you think this is a good idea or not?

### **2.1 Types Flat Files**

1. Google the differences between a `csv file`, a `JSON file`, and a `xml file`. 

2. Copy the text below into `Notepad` and save it as `cars.csv`

```
Year,Make,Model
1997,Ford,E350
2000,Mercury,Cougar
```
3. Transform the text into a `JSON file` and save it as a new file called `cars.json`. Make sure you keep both files. It is also up to you if you want to transform them manually or use a website.

4. Try to open both in Tableau. Do you notice any differences?


### **2.2 Connect to a database**

1. Open Tableau and connect to `Microsoft SQL Server`. Once the prompt opens, put in the following credentials:

- Server: `3.143.125.139`
- Authentication: `Use a specific username and password`
- Username: `SQL`
- Password: `SQL`

Leave everything else empty and unchecked. 

2. Explore the different databases and tables inside. Try to guess what each database is used for. For example, which ones are automatically generated.

### **2.3 Working with APIs**

1. Go to any browser and go to this site `https://openlibrary.org/search/authors.json?q=j%20k%20rowling`

2. Replace `j%20k%20rowling` by the name of any other author. 

Note: As you might have infered, `%20` is [HTML URL Encoding](https://www.w3schools.com/tags/ref_urlencode.ASP) for a space. There is at least one encoding for every character, but `%20` is the most common, since URLs cannot have spaces. Also, if `%20` feels a bit difficult to remember, you can also use `+`.

### **2.4 Web Data Connector**

1. Go to https://www.makeovermonday.co.uk/data/

2. Pick any dataset.

3. Open the link under the data column.

4. You will be redirected to [data.world](data.world). You can find all sorts of public datasets in here. Most of them are perfect for your final project.

5. Either create an account (you might be using this site more in the future) or use the following credentials to sign in:

- Username: @hc-analyzing-data
- Password: analyzing-data

5. Look for the `Open in app` button. The one with the three empty squares and the diamond at the top right of the dataset.

<img src="https://media.data.world/KVWgC7jTjWaDkId1ub4Y_Screen%20Shot%202018-04-20%20at%202.14.07%20PM.png" />

6. Follow the instructions and open it as a Web Data Connector in Tableau.

</details>