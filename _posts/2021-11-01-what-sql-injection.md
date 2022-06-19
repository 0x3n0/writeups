---
title: The Impact of Sql Injection Attacks in the Cybersecurity World
author: codericky
date: 2021-11-01 07:17:05 +0700
image: /assets/img/blogging/sql-injection.jpeg
categories: [Cybersecurity, what sql injection ]
tags: [sql injection attack, sql injection cheat sheet,
sql injection payloads, sql injection prevention,
sql injection tutorial, sql injection test,
sql injection types, sql injection examples,
sql injection login bypass, how to prevent sql injection,
blind sql injection, types of sql injection,
dvwa sql injection, owasp sql injection,
error based sql injection, basic sql injection, sql injection example]
---
SQL Injection is a technique in exploiting a way of **modifying sql commands**.

![sql injection](/assets/img/blogging/sql-injection.jpeg)

on the input form in the application that allows **an attacker to be able to submit syntax** into the application database.

SQL Injection can also be defined as a technique for exploiting security vulnerabilities in the **in the database layer** to get query data on an application.

## What Causes SQL Injection
SQL Injection can usually occur because the programmer (application developer) **does not implement a filter against the metacharacter** used in the sql syntax on the application input form.

so that the attacker can input the **metacharacter** into instructions on the application system to access a database.

In addition, SQL Injection attacks can also occur, if the personnel at the back end **do not implement or do not set up Web** .

Application Firewall (WAF) or an Intrusion Prevention System a(IPS) in a network architecture properly, so that **in the database** applications can be accessed directly from vulnerabilities found.

SQL Injection attack is an attack method by doing **code injection**, used to attack data-based applications. This vulnerability allows hackers **entering artificial input** to interfere with **an application interaction** with databases on the back-end.

the cracker may be able to get **arbitrary data** from the application, which tampered with its logic, or run a **command on the server** database itself.

## There are several types of SQL Injection attacks, including:

1. Union-Based SQL Injection
It is the most popular type of **SQL Injection attack**. This type of attack uses a UNION statement, which is a **combination of two statements**, to get data from the database.

2. Error-Based SQL Injection
The attack type in **SQL Injection is the simplest**, and the only problem with this type of attack is that it can only run on a Microsoft SQL Server.

This attack method, will make the application show an error when accessing the database. From this error the attacker will learn system information such as database, `database version`, `operating system`, and `etc'.

3. Blind SQL Injection
Blind SQL Injection is the most difficult type of SQL Injection attack. In this attack, **no error messages** are received from a database. **Almost the same as other SQL Injection attacks**, what makes it different is how the data is retrieved from the database.

# There are 2 Types of Blind SQL Injection:

1. Content-based Blind SQL Injection
The attacker will do and try **to verify the database** is vulnerable to Blind SQL Injection by comparing **results from different queries returned** with `TRUE` or `FALSE`.

2. Time-based Blind SQL Injection
The attacker will be able to instruct a database to perform a time-intensive operation. If in the web site **does not return a response** immediately, **means the web application is vulnerable to Blind SQL Injection attacks**.

## Anticipate Sql Injection Attacks
1. Provide encryption and **lock on database**
To secure data from attackers, you can use encryption for your database to be safe.

You can store data **which is credential** separately to make it difficult for an attacker to perform SQL Injection.

In addition, you can also lock the system database so that SQL Query cannot be accessed **through user pages** website.

You can provide a limitation that not all users can **do access to the table**. Namely by locking a very vital table.

2. Limitation of access rights
The purpose of granting access rights restrictions to users is to **prevent SQL Injection**. Never log into the database **using an admin access** as root. However, you can use predefined privileged access to limit the scope on the system**.

1. Provide user input validation
You can **perform input filters on user display forms** to prevent SQL Injection from occurring. Filters that you can apply such as filter types,

length, input format, and so on. Thus, only input that passes validation can be used in **a database query**.

4. Using Parameterized Query
Parameterized Query is a query that uses a marker, where this `marker` or `parameter` will be given the time value in the query `run` or `execute`.

This method is a simple way that can be done **to prevent SQL Injection**. Parameterized will define the entire SQL code before sending it to the query layer.

Every database must be able and able to recognize an input entered by the user, which is included in the category of `SQL code` or `user data`.

Thus, the attackers **can't change the contents of the query**. Even though it has entered the SQL code while doing the input.

## Conclusion
The explanation above we have learned, about understanding what is sql injection, several types of sql injection attacks, types of blind sql injection attacks, and anticipating sql injection attacks.

