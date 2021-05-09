## T2A1 - Workbook 2 
---
### Brief 
The ACME Corporation is interested in building a marketplace web application (app) using Rails for one of it’s product lines. To help it choose the vendor who will undertake the project they have released a RfQ. As an aspiring junior dev at an up and coming Sydney software startup (CAx-Dev) your manager has assigned you to assist with preparation of the RfQ response.

#

### Q1:
#### Describe the architecture of a typical Rails application

On every web application used today, the interactions between programmes, databases, and middleware systems ensures that many applications can run at the same time. For example; when a user clicks on a home button it requests for that particular web address. It then makes a request for the specific web address. As a response to the request, the server sends files to the browser. After that, the browser runs certain files in order to display the requested page. 

One of the most common architectural patterns in a web application is the Model View Controller (MVC). It's used to build maintainable GUI systems, and it's available in almost every language. 

- Model: Handles all application logics where data is saved and how data should react to certain commands. 

- View: The part of the software that controls what the user sees. This section of the software displays data obtained from the Model and on certain occation, from the controller. 

- Controller: Awaits for user's commands (inputs) to inform the other two sections of the software to make the necessary changes. 

Ruby on Rails framework is an example that uses conventions and assumptions. This convention eliminates configuration code for ease of use on the language writing less code. 

![flowchar](/img/flowchart.png)

#

### Q2:
#### Identify a database management system (DBMS) commonly used in web applications (including Rails) and discuss the pros and cons of this database

PostgreSQL, also known as "Post-Gress," is a free and open-source relational database management system (RDBMS) that is widely used in the industry. It provides a large number of functions to its users. These  benefits programmers in the development of new software, administrators in the protection of data integrity, and developers in the creation of resilient and stable environments. PostgreSQL allows its users to manage data regardless of the size of the database. 

PostgreSQL also available on multiple popular used operating systems such as MacOS X, Windows and Linux. It is simple to update or extend due to its open source design. Users can also define their own data types, create custom functions, and even write code in another programming language without having to recompile the database. 

Big Tech industries which uses PostgreSQL includes;
- Apple
- Spotify
- Instagram
- Skype

The Pros and Cons of PostgreSQL:

#
| Pros  | Explanation          |
| ------- | ---------------- |
| Data Types    | supports a wide set of Data Types. Besides, users can create their own custom data type using CREATE TYPE SQL command.  |
| Data Integrity | The best needed constraints are supported in PostgreSQL like UNIQUE, NOT NULL, Primary Keys, Foreign Keys. |
| Data Size | It can handle a lot of data with an unlimited database size. |

| Cons  | Explanation          |
| ------- | ---------------- |
| Open Source | Being an open source project has many advantages, but it also has many disadvantages. Because it is an open-source software, there is no warranty or security in using it, and because it is run by the community, it may lack many of the user-friendly features that we have come to expect from other applications. | 
| Speed | Compared to other Database Management Systems, PostgreSQL specializes in dealing with large and challengeing databses whilst other focuses on speed and reliability. |

#

### Q3:
#### Discuss the implementation of Agile project management methodology.

Agile project management is an iterative project management methodology that focuses on splitting complex projects down into smaller, more manageable activities that are performed in brief iterations during the project life cycle. Agile teams are better able to complete work quicker, adjust to evolving project requirements, and streamline their processes. 

The steps in the Agile Methology:

Step 1. Project Planning

Understand the ultimate target, the importance to the company or customer, and how it will be accomplished.

Step 2. Product roadmap creation

A roadmap is a list of features that will be included in the final product,which is an important part of the Agile planning stage.

Step 3. Release Planning

In a Agile Methology, each feature are released every end of each cycle since the projects are uses shorter development process called (sprints). Where there are short itiration between one to two weeks to complete.

Step 4. Sprint Planning 

Before each sprint starts, the stakeholders must hold a sprint planning meeting to decide what each individual will accomplish during that sprint, how it will be accomplished, and evaluate the task load.

Step 5. Daily Stand-ups

To assist the team in completing their tasks during each sprint and determining whether any changes are required, daily 15min discussions are made, briefly talking about what has been accomplished previous day and what they will be working on on the day.

Step 6. Sprint review and retrospective 

The team will hold two meetings after each sprint ends: the first will be a sprint summary with project stakeholders to show them the finished product. This is a crucial aspect of maintaining open lines of communication with stakeholders.

#

### Q4:
#### Provide an overview and description of a standard source control workflow

The process of monitoring and handling code changes is known as source control (or version control). The aim of source control is to keep track of revisions and share changes between groups of files. The files are typically text, but they may also be binary, images, or other types of files.

There are mainly two types of version control:

Centralized version control

![Centralized_Version_Control](/img/centralize.png)

a single server containing all the versioned files, and a variety of clients checking out files from that central location.  

![CDistributed_Version_Control](/img/distribute.png)

Users don't only download the most recent version of the files; they also mirror the archive in its entirety, including its entire history. As a result, if any server goes down and these systems were collaborating via it, any of the client repositories can be copied back up to the server to get it back online. Every clone is a complete backup of all data.

#

### Q5: 
#### Provide an overview and description of a standard software testing process (e.g. manual testing)

Software testing is a technique for determining whether the real software product meets the intended specifications and ensuring that it is defect-free. It entails the use of manual or automated methods to test one or more properties of interest by executing software/system components. In comparison to real specifications, software testing's aim is to find bugs, holes, and missing requirements.

Manual testing is a form of software testing in which test cases are manually performed by a tester instead of using automated tools. The aim of manual testing is to find bugs, problems, and flaws in a software application. Manual software testing is the most basic of all testing methods, and it aids in the discovery of important vulnerabilities in software applications.

Automation Testing, also known as Test Automation, is a software testing technique that involves the execution of a test case suite using special automated testing software methods. Manual testing, on the other hand, is carried out by a person sitting in front of a monitor, carefully carrying out the test steps.

#

### Q6:
#### Discuss and analyse requirements related to information system security and how they relate to the project

Businesses has the obligation to protect its customers from security breaches to prevent confidential information out in the public. Each requirement to prevent any issues must detect and quantify possible weaknesses in a system such that risks can be encountered and the system does not stop working or be abused. 

Authentication

Unforgeable digital certificates from a trusted authority are the best protection against being fooled by an imposter in online commerce. While anyone can create digital certificates for themselves, a trusted authority requires real-world proof of identity before issuing a digital certificate and verifies its validity. The main web browser and email client applications can only accept and trust certificates issued by trusted authorities. Physical tokens can be used to provide authentication in certain cases (such as a drivers license).

Authorization 

A individual or computer system may use authorisation to see if anyone has the authority to request or authorise an action or details. Authentication in the physical world is normally accomplished by signature-required forms or locks that only allowed individuals have the keys to. In the project The server may obtain a digital certificate from the user's browser in order to identify the user and decide whether or not they should be granted access to the information based on the server's permission rules.

Integrity

Integrity of information ensures that the communication received has not been altered and the data represented in the databse is accurate. An example in the project is If someone receives confidential information over the internet, he needs to make sure it not only comes from who he thinks it to come from (authentication), but also that it hasn't been altered by a hacker and its contents haven't been changed.

#

### Q7:
#### Discuss common methods of protecting information and data and how you would apply them to the project

Session Hijacking

Is essentially when a user provides authentication information to gain access. The web application checks them and stores the corresponding user id in the session hash called cookies servers. Anyone who steals a cookie from another user has the potential to use the web application as that user, with potentially serious consequences. In the project, rails this can be done by having the application's config file, always force SSL connections:
```ruby 
config.force_ssl = true
```

Furthermore, rails provide encrypted cookie jar to provide a secure, encrypted location to store session data
```ruby
ActionDispatch::Session::CookieStore
```

Session Fixation

The aim of this attack is to fix a user's session ID, which is known to the attacker, and force the user's browser to use it. As a result, the intruder does not need to steal the session ID later. The most powerful countermeasure is to generate a new session identifier after a successful login and declare the old one invalid. An attacker would be unable to use the set session identifier in this manner. In the project, the following code can be implemented in ruby rails
```ruby
reset_session
```
However there are gems which can do this automatically, 'Device' being one of the most used gem.

#

### Q8:
#### Research what your legal obligations are in relation to handling user data and how they can be met for the project

Many businesses must, as a minimum, comply with the National Privacy Principles set by the Australian _Privacy  Act  1988_. This ensures customers' personal information will not be used maliciously. In the project, customers has the right to know what information a company has on them and to get the information corrected if it is inaccurate, out of date, or incomplete. A company must take appropriate measures to warn customers that personal information is being collected and why it is being collected. Since users are giving credit card and home address information to the company. 

Conclusion of contract let customers know the purpose they require the product or service they wish to achieve. Procedures which the project can implement are:
- 'terms and conditions' when a customer joins and or uses the service.
- Identify and correct any errors 
- confirm, accept or reject products.

#

### Q9:
#### Describe the structural aspects of the relational database model. Your description should include information about the structure in which data is stored and how relations are represented in that structure.

A relational database is a type of database that employs a framework that enables customers to locate and access data in the context of other data in the database. A relational database's data is often arranged into tables. The data structure of a relation database model includes data types, indexes, and views. The data tables are used to store information about objects, with each row containing a unique key and each column containing data object attributes. record will have a primary key that is special to the table, as well as international keys that reflect relationships between records.

There are 3 types of relational that a data can be represented on in a relation database model.
1. One-To-One Relationship
- One record in a table is associated with one and only one record in another table
2. One-To-Many Relationship
- One record in a table can be associated with one or more records in another table.
3. Many-To-Many Relationship
- Occurs when multiple records in a table are associated with multiple records in another table.

#

### Q10
#### Describe the integrity aspects of the relational database model. Your description should include information about the types of data integrity and how they can be enforced in a relational database.

Data integrity applies to the data's protection and security in terms of regulatory enforcement, such as Data privacy and compliance (GDPR) compliance. It is kept up to date by a set of procedures, guidelines, and specifications that were put in place during the design phase. The information contained in a database will remain complete, accurate, and reliable no matter how long it is stored or how often it is accessed if the data integrity is secure. In the project the Logical Integrity will mostly likely be used.

Types of Data Integrity include:

Entity integrity

To insure that data isn't specified more than once and that no field in a table is null, relies on the creation of primary keys, or unique values that mark pieces of data. It's a characteristic of relational databases, which store information in tables that can be connected and used in a number of ways.

Referential integrity

A collection of procedures for ensuring that data is maintained and used consistently. Only necessary modifications, additions, or deletions of data are made, thanks to rules embedded in the database's layout on how foreign keys are used.

Domain Integrity

The set of processes that ensures that each piece of data in a domain is accurate. A domain is a collection of suitable values that a column may contain in this context.

#

### Q11
#### Describe the manipulative aspects of the relational database model. Your description should include information about the ways in which data is manipulated (added, removed, changed, and retrieved) in a relational database.

When a developer performs any CRUD action on a data object in a relational database model, the SQL database language is used to modify aspects of the database. When a developer performs any CRUD action on a data object in a Rails programme, the SQL commands are executed by the Active Record. This action can be done by these actions; SELECT, INSERT, UPDATE, DELETE. 

SELECT - is used to retrieve rows selected from one or more tables.
```ruby
SELECT product_name /*The column you want to see...*/
FROM product; /*...from the table it belongs.*/
```

INSERT - inserts new rows into an existing table.
```ruby
INSERT INTO product (product_code, product_name, unit_price)
VALUES (101, "coffee", 4.50);
```

UPDATE - updates columns in existing table rows with new values.
```ruby
UPDATE product
SET product_name="cantaloupe"    /*New value*/
WHERE product_name="melon";    /*Specific value to overwrite*/
```

DELETE - deletes rows from table_name that satisfy the condition given by where_definition, and returns the number of records deleted.
```ruby
DELETE FROM product
WHERE product_name="coffee"; /*Row to delete*/
```

#

### Q12
#### Conduct research into a marketplace website (app) and answer the following parts:  
#### a. List and describe the software used by the app.
#### b. Describe the hardware used to host the app.
#### c. Describe the interaction of technologies within the app
#### d. Describe the way data is structured within the app
#### e. Identify entities which must be tracked by the app
#### f. Identify the relationships and associations between the entities you have identified in part (e)
#### g. Design a schema using an Entity Relationship Diagram (ERD) appropriate for the database of this website (assuming a relational database model)

For this research, I have chosen Ebay which sells various goods from small businesses to individuals

#

A. List and describe the software used by the app.
![Csoftware1](/img/software1.png)
![Csoftware2](/img/software2.png)

Javascript - JavaScript is the Programming Language for the Web.JavaScript can update and change both HTML and CSS.

Node.js - Node.js is an open-source, cross-platform, back-end JavaScript runtime environment

#

B. Describe the hardware used to host the app.

Ebay is build on its own servers using Point of Presence (PoP) strategy, decentralizing the cluster of data centers scattered accross the US. They are also using NuData, a geo-distributed, fault-tolerant object and data store In the long run, this will allow eBay to disperse data globally provide data isolation solutions for countries that need them.

#

C. Describe the interaction of technologies within the app





























