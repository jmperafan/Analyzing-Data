---
theme: default
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.jpg')
marp: true

---

# **Analyzing Data**
### A Practical Guide

![bg left:40% 80%](https://www.rug.nl/education/honours-college/news/20190712guf100!attachment?c=images/news-image-big.jpg)

github.com/jmperafan/analyzing-data

---

<!-- header: 'Sep 21 - Introduction to Analytics' -->
# **Introduction to Analytics**

### Learning objectives
- Gain a conceptual understanding of data and analytics.
- Learn the most common career paths for data professionals.
- Be exposed to some of the common data challenges in organizations.
- Become acquainted with [Tableau](https://www.tableau.com/).

---

# **What is Analytics?**

![bg left](https://lh3.googleusercontent.com/MzcojAroNPS2Uno2E73nbUoKULgrVW6UbAyJvQOpwtHKAqnrfo9krb1SS8WAYkqw5pmzAlI1EurwSyg1H8Yev8zmvdNostmUwBGL=s2500)

Systematic computational analysis of data used for the:
- Discovery
- Interpretation
- Communication 

of *meaningful* patterns in data.

---

# **What is data?**

Information in binary digital form. 
**Anything** can be enconded as a 1 or 0.

![bg right](https://repository-images.githubusercontent.com/189982674/1639be00-dbe8-11ea-9ccb-50f536b433b2)

---

<!-- 
    Discussion Exercise:
    The objective of this exercise is to ask students to reflect on their digital footprint and be exposed to some of the most common data problem that companies face.
-->

# **Go Full Stalker**
![bg left](https://miro.medium.com/max/1400/1*Wa9c49hXvSQOUdGCMG0rBA.png)

Imagine your objective is to create a digital trail of somebody's day. Make it at detailed as possible. Your exercise now is to think:

1. What type of data could you collect?
2. What problems would you run into?

---

<!-- Not completed -->
# **Data Jobs**
![w:32 h:32](/slides/diagrams/data_jobs.png)

---

# **What is Tableau?**
![bg right](https://cdnl.tblsft.com/sites/default/files/pages/platform-3-800x5002x_1.jpg)

Tableau helps people see and understand data. 
- Stunning visuals in seconds. 
- Makes exploratory  analysis fun.
- Very easy to learn.

---

<!-- Not completed -->
# **About this course**
Here is what you should know about the course:

1. Everything is on Github.
2. We will be using Tableau.
3. There is a final assignment.

---

<!-- header: '28 Sep - Storing & Extracting Data' -->
# **Storing & Extracting Data**
### Learning objectives
- Exposure to the most common data storage ecosystems.
- Learn the most common challenges around ingestion, storage, and extraction of data.
- Practice loading different types of datasources in Tableau.

---

# **Data Trends**
![bg fit right](https://i.redd.it/fqii2tufdgwz.jpg)

Back in 70's, when the first databases were invented, storing data was absurdly expensive. 

That has changed and consequently we are capturing exponential amounts of data.

---

# **Where is the data?**
![bg left](https://www.talk-business.co.uk/wp-content/uploads/2015/02/shutterstock_300344546.jpg)

Data is generally scattered:
- `Flat files`
- `Databases`
- `Data Warehouses`
- `Data Lakes`
- `Source systems`
- `APIs`

---

# **Flat Files**
![bg right](https://www.weirdgeek.com/wp-content/uploads/2018/12/Reading-Most-Common-File-Formats-in-Data-Science.png)

Common formats include `.csv`, `.txt`, `.xlsx`, `.json`, `xml`, `.avro`, `.parquet`. 


\+ Flexibility.
\- Collaboration.
\- Security.
\- Scalability.

---

# **Databases**
![bg right](https://upload.wikimedia.org/wikipedia/commons/thumb/9/94/MediaWiki_1.28.0_database_schema.svg/1200px-MediaWiki_1.28.0_database_schema.svg.png)

Databases are an attempt to professionalize data storage. They are composed of spreadsheet-like tables that are related to each other. 

\+ Collaboration.
\+ Security.
\- Flexiblity.
\- Scalability.
\- Tabular.

---

# **Data Warehouse**
![bg right](https://miro.medium.com/max/878/0*OU8MGyXkSlZvHHr7.)

Data warehouse look and feel like a database. But they are optimized for analytics (instead of powering an application).

\+ Collaboration.
\+ Security.
\+ Scalability.
\- Flexibility.
\- Tabular.

---

# **Data Lake**
![bg right](https://d1.awsstatic.com/Data%20Lake/what-is-a-data-lake.c3917cc3e6af77037a814c5aeb7cec1de7f89eb9.PNG)

Data lakes are a cheaper, more flexible of data warehouses. Data doesn't need to be tabular or relational anymore. But it can get messy.

\+ Collaboration.
\+ Scalability.
\+ Flexibility.
\- Order.

---

# **Source Systems**
![bg right](https://2s7gjr373w3x22jf92z99mgm5w-wpengine.netdna-ssl.com/wp-content/uploads/2020/09/FiveTran.png)

Source system is any system that captures data. You generally don't want it to live here.

\- Flexibility.
\- Centralization.

---

# **APIs**

![bg right](https://www.seobility.net/en/wiki/images/f/f1/Rest-API.png)

APIs can be used as a secure interface to allow anybody to query data.

\+ Automation.
\+ Security.

---

<!-- header: '28 Sep - Storing & Extracting Data' -->
