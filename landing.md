---
title: UNIT 3
layout: landing
image: assets/images/SQL.png
nav-menu: true
---

<!-- Main -->

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Learning Portfolio: Database Systems</title>
    <style>
        body { font-family: Arial, sans-serif; line-height: 1.6; margin: 20px; padding: 20px; }
        h1, h2, h3, h4 { color: white; }
        code { background: black; color: white; padding: 3px 5px; border-radius: 3px; }
        pre { background: black; color: white; padding: 10px; border-radius: 5px; overflow-x: auto; }
    </style>
</head>

<body>
    
<h2>Lesson 6: Null Values, Aggregate Functions, and Grouping Data</h2>
    
<h3>Handling Null Values in SQL</h3>
    <p>Null values signify missing or unknown data, making their proper handling essential for maintaining data integrity and accuracy.</p>
    <ul>
        <li><strong>Why Are Nulls Important?</strong></li>
        <ul>
            <li>Null values are distinct from zero or empty strings.</li>
            <li>Any mathematical operation involving NULL results in NULL.</li>
            <li>Comparisons with NULL yield an “unknown” result instead of true/false.</li>
        </ul>
        <li><strong>Techniques for Managing NULL Values in Queries:</strong></li>
        <ul>
            <li>Use <code>IS NULL</code> and <code>IS NOT NULL</code> to filter null values.</li>
            <li>Apply <code>COALESCE(value, replacement_value)</code> to substitute NULL with a default value.</li>
            <li>Use <code>NULLIF(value1, value2)</code> to return NULL when both values are identical.</li>
        </ul>
    </ul>
    <pre><code>SELECT * FROM employees WHERE salary IS NULL;</code></pre>
    
    <h4>Handling NULL in Aggregate Functions</h4>
    <p>Aggregate functions typically disregard NULL values, except for COUNT(*), which counts all rows including NULLs.</p>
    <pre><code>SELECT COUNT(*) AS total_rows, COUNT(salary) AS non_null_salaries FROM employees;</code></pre>

<h3>Aggregate Functions in SQL</h3>
    <p>Aggregate functions summarize data across multiple rows, aiding in efficient data analysis.</p>
    <pre><code>SELECT department, COUNT(*) FROM employees GROUP BY department;</code></pre>

<h3>Grouping Data with GROUP BY and HAVING</h3>
    <p>The <code>GROUP BY</code> clause groups records based on a specified column, while <code>HAVING</code> filters aggregated results.</p>
    <pre><code>SELECT department, AVG(salary) 
FROM employees 
GROUP BY department 
HAVING AVG(salary) > 50000;</code></pre>
    
<h2>Lesson 7: Nested Subqueries and Advanced SQL</h2>
    
<h3>Nested Subqueries</h3>
    <p>Subqueries are queries embedded within another SQL query, enabling more intricate data retrieval.</p>
    <pre><code>SELECT course_id FROM section WHERE semester = 'Fall' 
AND course_id IN (SELECT course_id FROM section WHERE semester = 'Spring');</code></pre>

    <h3>Correlated Subqueries</h3>
    <p>Unlike regular subqueries, correlated subqueries execute once for each row processed by the outer query.</p>
    <pre><code>SELECT name, department, salary 
FROM employees e1
WHERE salary > (SELECT AVG(salary) FROM employees e2 WHERE e1.department = e2.department);</code></pre>

<h2>Lesson 8: Database Modifications</h2>
    
<h3>Database Modification Operations</h3>
    <ul>
        <li><strong>Inserting Data:</strong> Adding new records into a table.</li>
        <pre><code>INSERT INTO students (id, name, age) VALUES (101, 'Alice', 22);</code></pre>
        <li><strong>Deleting Data:</strong> Removing records based on specific conditions.</li>
        <pre><code>DELETE FROM students WHERE age < 18;</code></pre>
        <li><strong>Updating Records:</strong> Modifying existing data within a table.</li>
        <pre><code>UPDATE employees SET salary = salary * 1.05 WHERE department = 'HR';</code></pre>
    </ul>

<h2>Advanced SQL Concepts</h2>
    <h3>Window Functions</h3>
    <p>Window functions allow calculations across a subset of rows while retaining individual row details.</p>
    <pre><code>SELECT name, salary, RANK() OVER (ORDER BY salary DESC) AS rank FROM employees;</code></pre>

    <h3>Set Operations</h3>
    <p>Set operations, including <code>UNION</code>, <code>INTERSECT</code>, and <code>EXCEPT</code>, facilitate dataset comparison and combination.</p>
    <pre><code>SELECT name FROM students
UNION
SELECT name FROM alumni;</code></pre>
    
    <p>To find students who are also alumni:</p>
    <pre><code>SELECT name FROM students
INTERSECT
SELECT name FROM alumni;</code></pre>
    
    <p>To identify students who are not alumni:</p>
    <pre><code>SELECT name FROM students
EXCEPT
SELECT name FROM alumni;</code></pre>

<h2>Reflections and Insights</h2>
    <p>Mastering SQL has been a transformative journey. Initially, handling NULL values and subqueries posed challenges, but with persistence, these concepts became second nature. Exploring aggregate functions, GROUP BY, and set operations has deepened my understanding of database management.</p>

<h2>Conclusion</h2>
    <p>This portfolio encapsulates my growth in database systems, spanning fundamental SQL operations to advanced functionalities. Moving forward, I aspire to delve into transactions, indexing, and optimization techniques to enhance efficiency and scalability in database management.</p>

</body>
