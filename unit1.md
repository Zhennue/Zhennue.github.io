---
layout: page
title: UNIT 1
image: assets/images/pic01.png
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Unit 1</h1>
		</header>

<!-- Content -->
<h2 id="content">Lesson 1</h2> <br>

<h3>What is a Database System?</h3>
<p>A database system is a structured collection of data managed through a Database Management System (DBMS). It ensures efficient storage, retrieval, and management of data.
Key Components:Data: Collection of facts.
Database: Organized data stored electronically.
DBMS: A system to manage databases.
Database System: Combination of database and DBMS.</p>
<div class="row">
	<div class="6u 12u$(small)">
		<h3>Advantages of Database Systems</h3>
		<p>✅ Data Consistency - Reduces duplication and maintains uniformity.<br>
		✅ Scalability & Flexibility - Adapts to changing needs.<br>
		✅ Better Security - Ensures controlled access.<br>
		✅ Improved Data Retrieval - Faster and structured access to information.<br>
		✅ Data Abstraction - Simplifies complex data structures.</p>
	</div>
	<div class="6u$ 12u$(small)">
		<h3>Disadvantages of File-Processing Systems:</h3>
		<p>❌ Data redundancy and inconsistency<br>
		❌ Difficulty accessing data<br>
		❌ Integrity and security issues<br>
		❌ Data isolation and atomicity problems<br>
        📌 Example: Student registration at a college involves multiple physical forms, bank transactions, and manual record-keeping, making the process inefficient and prone to errors.</p>
	</div>
	<!-- Break -->
	<div class="4u 12u$(medium)">
		<h3>Why Do We Need Database Systems?</h3>
		<p>Traditionally, organizations relied on manual record-keeping or file-processing systems, leading to several challenges.</p>
	</div>
	<div class="4u 12u$(medium)">
		<h3>Real-World ApplicationsDatabase systems are widely used in various fields:</h3>
		<p>Banking & Finance - Transaction processing, customer records. 🏦<br><br>
		Social Media - Managing vast user data. 📱<br><br>
		Sales & E-commerce - Inventory tracking, customer orders. 🛒<br><br>
		Navigation Systems - Location-based data. 🗺️<br><br>
💡     "Data is the new gold." A well-managed database system ensures efficient handling of valuable data resources.</p>
	</div>
	<div class="4u$ 12u$(medium)">
		<h3>Evolution of Database Systems</h3>
		<p>Database systems have evolved from file-based storage to advanced DBMS platforms with powerful data analytics and cloud storage capabilities. More on Database History<br></p>
	</div>
</div>

<hr class="major" />

<!-- Elements -->
<h2 id="elements">Lesson 2</h2>
<div class="row 200%">
	<div class="6u 12u$(medium)">

<!-- Text stuff -->
<h3>Introduction to Database & DBMSDatabase: </h3>
<p>A structured collection of related data.
DBMS (Database Management System): Software that allows users to create, manage, and manipulate databases.
Key Difference: A database stores data, while a DBMS helps in accessing and managing it efficiently.</p>
<hr />
<h3>Views of Data</h3>
<hr />
<p>A DBMS supports defining, creating, querying, updating, and administering databases based on data models.
Types of Data ModelsEntity-Relationship (ER) Model
Semi-Structured Data Model
Object-Based Data Model
Relational Model (focus for this module)
</p>



<h3>Data Abstraction Levels</h3>
<dl>
	<dt>Physical Level</dt>
	<dd>
		<p>How data is stored.</p>
	</dd>
	<dt>Logical Level</dt>
	<dd>
		<p>What data is stored and how it’s related.</p>
	</dd>
	<dt>View Level</dt>
	<dd>
		<p>Provides different views for users.</p>
	</dd>
</dl>



<!-- Blockquote -->
<h3>Fun Facts</h3>
<blockquote>Did you ever notice that all the letters of the word database are typed with the left hand? 
Interesting right? Now, the layout of QWERTY keyboard was designed, among other things, to facilitate the better use of both the hands. Therefore, it pretty much follows that writing about databases is not only unnatural, but also a lot harder than it seems.</blockquote>




</div>
<div class="6u$ 12u$(medium)">

<!-- Image -->
<h3>Image</h3>

<span class="image fit"><img src="{% link assets/images/What-is-Database-2.jpg.webp %}" alt="" /></span>
<div class="box alt">
	<div class="row 50% uniform">
		<div class="4u"><span class="image fit"><img src="{% link assets/images/pic1.png %}" alt="" /></span></div>
		<div class="4u"><span class="image fit"><img src="{% link assets/images/pic2.png %}" alt="" /></span></div>
		<div class="4u$"><span class="image fit"><img src="{% link assets/images/Semi-structured-Data.webp %}" alt="" /></span></div>
	</div>
</div>

<h4>Database Engine & System Architecture</h4>
<p><span class="image left"><img src="{% link assets/images/DBMS archi.png %}" alt="" /></span>Database Engine: Manages storage, transactions, and queries.<br>
Components of DB Engine: <br>
Storage Manager: Interfaces with stored data.<br>
Query Processor: Interprets SQL commands.<br>
Transaction Management: Ensures consistency and recovery.</p>
<p><span class="image right"><img src="{% link assets/images/SQL-Commands-2018664638-1576589804123.png %}" alt="" /></span>SQL and Database LanguagesDDL (Data Definition Language): Defines database schema.<br>
DML (Data Manipulation Language): Allows queries and updates.</p>

