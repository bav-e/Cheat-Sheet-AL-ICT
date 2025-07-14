# **Final Plan for Lesson 10 Cheat Sheet: Web Development**

### **The Goal**

To create a "Syntax-First" reference sheet that is fully aligned with the provided practical guide. It will focus on providing quick, easy-to-find code snippets and concepts for the most common tasks in HTML, CSS, and PHP, reflecting the A/L standard.

### **The Structure: "From Frontend to Deployment"**

The cheat sheet will be structured into three logical parts, covering the entire web development lifecycle from creating the user interface to publishing the final product.

## **Content List for the Cheat Sheet**

### **Part 1: Frontend Development (HTML & CSS)**

*This will be a detailed quick reference for building the user interface, using the exact tags and syntax emphasized in the guide.*

* **HTML Core Structure & Tags:**  
  * **Basic Structure:** \<\!DOCTYPE html\>, \<html\>, \<head\>, \<title\>, \<body\>.  
  * **Comments:** \<\!-- comment \--\>.  
  * **Text Formatting:** \<h1\>-\<h6\>, \<p\>, \<br\>, \<b\>, \<i\>, \<u\>.  
  * **Links & Images:**  
    * \<a\> with href for internal (relative) and external (absolute) links.  
    * \<img\> with src and alt attributes.  
  * **Lists:**  
    * \<ul\> (Unordered), \<ol\> (Ordered, with start attribute), and nested lists.  
  * **Tables:**  
    * Core Tags: \<table\> (with border attribute), \<tr\>, \<th\>, \<td\>.  
    * Structural Tags: \<thead\>, \<tbody\>, \<tfoot\>.  
    * Cell Merging: colspan and rowspan attributes.  
  * **Multimedia:** \<audio\> and \<video\> tags with the src attribute.  
* **CSS Core Concepts:**  
  * **Syntax:** selector { property: value; }.  
  * **Selectors:** Element (p), Class (.my-class), ID (\#my-id), and Compound selectors.  
  * **Insertion Methods:**  
    * Inline (style attribute).  
    * Internal (\<style\> tag).  
    * External (\<link\> tag and @import directive).  
  * **Common Properties:**  
    * **Text/Font:** color, font-size, font-family.  
    * **Background:** background-color, background-image.

### **Part 2: Backend Development (PHP & MySQL)**

*This section focuses on making the website dynamic, using the specific syntax from the guide.*

* **PHP Basics:**  
  * **Embedding:** \<?php ... ?\>.  
  * **Variables & Output:** $variable \= "value";, echo $variable;.  
  * **Comments:** // (single-line), /\* ... \*/ (multi-line).  
  * **Control Structures:** if...elseif...else, switch, while, do...while, for.  
  * **Array Sorting Functions:** A note on key functions like sort(), rsort(), asort(), ksort().  
* **HTML Forms (The bridge between user and server):**  
  * \<form\> tag with action="...php" and method="post|get".  
  * **GET vs. POST:** GET shows data in URL; POST hides it in the request body.  
  * **Input Elements:** \<input type="text"\>, type="password", type="radio", type="checkbox", type="submit".  
  * **Other Form Elements:** \<textarea\>, \<select\>, \<label\>, \<fieldset\>.  
* **PHP & MySQL (Connecting to a Database):**  
  * **Connection Methods:** A note on the two methods shown: MySQLi (object-oriented) and MySQLi (procedural).  
  * **Typical DB Operation Flow (Procedural Example):**  
    1. $link \= mysqli\_connect(...) \- Establish connection.  
    2. $sql \= "INSERT INTO ..." \- Formulate the SQL query.  
    3. mysqli\_query($link, $sql) \- Execute the query.  
    4. $row \= $result-\>fetch\_assoc() (for SELECT) \- Process results.  
    5. mysqli\_close($link) \- Close the connection.  
  * **Retrieving Form Data in PHP:** Using the superglobals $\_POST\['input\_name'\] or $\_GET\['input\_name'\].

### **Part 3: Publishing & Key Concepts**

*This will be a smaller, conceptual section for quick revision.*

* **Website Types:** Static vs. Dynamic.  
* **Core Concepts:** Client-Server Model, URL components (protocol, domain, path).  
* **Publishing & Hosting:**  
  * Local vs. Internet Publishing.  
  * Key Terms: ISP, Web Hosting, Domain Name.  
* **Website Maintenance:** A note on the importance of regular backups, security updates, and monitoring site statistics.  
* **Web Authoring Tools:** A brief note that tools like Dreamweaver can generate code automatically.