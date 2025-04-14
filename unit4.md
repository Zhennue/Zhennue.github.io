---
title: UNIT 4
layout: landing
image: assets/images/9a.jpg
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

<h2>Lesson 9: Transactions and Concurrency Control</h2>

<h3>Transactions</h3>
<p>A transaction is a logical unit of work that contains one or more SQL statements. Transactions ensure data integrity through the ACID properties:</p>
<ul>
    <li><strong>Atomicity:</strong> Ensures all operations in a transaction are completed; otherwise, none are.</li>
    <li><strong>Consistency:</strong> Ensures the database transitions from one valid state to another.</li>
    <li><strong>Isolation:</strong> Ensures transactions do not interfere with each other.</li>
    <li><strong>Durability:</strong> Ensures that once a transaction is committed, it remains so, even in case of a system failure.</li>
</ul>

<h3>Concurrency Control</h3>
<p>Controls the simultaneous execution of transactions to ensure database consistency.</p>
<ul>
    <li><strong>Problems:</strong> Lost update, dirty read, non-repeatable read.</li>
    <li><strong>Techniques:</strong> Lock-based, timestamp-based, and optimistic concurrency control.</li>
</ul>

<pre><code>BEGIN TRANSACTION;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;</code></pre>

<h2>Lesson 10: Recovery Systems</h2>

<h3>Database Recovery</h3>
<p>Recovery ensures the database is restored to a consistent state after a failure.</p>
<ul>
    <li><strong>Types of Failures:</strong> Transaction failure, system crash, disk failure.</li>
    <li><strong>Recovery Techniques:</strong> Log-based recovery, checkpointing, shadow paging.</li>
</ul>

<h3>Log-Based Recovery</h3>
<p>Uses a log to record all database modifications. Ensures REDO and UNDO operations can be performed.</p>
<pre><code>WRITE-AHEAD LOGGING (WAL)
- All log records must be written to disk before the actual data is written.
- Ensures durability and atomicity.</code></pre>

<h2>Lesson 11: Database Security</h2>

<h3>Security and Authorization</h3>
<p>Ensuring data is protected from unauthorized access or malicious actions.</p>
<ul>
    <li><strong>Database Security Measures:</strong></li>
    <ul>
        <li>Access Control (GRANT, REVOKE)</li>
        <li>Encryption (data-at-rest, data-in-transit)</li>
        <li>Auditing and monitoring</li>
    </ul>
    <li><strong>SQL Commands:</strong></li>
    <pre><code>GRANT SELECT ON students TO user1;
REVOKE SELECT ON students FROM user1;</code></pre>
</ul>

<h3>Threats to Database Security</h3>
<ul>
    <li>SQL Injection</li>
    <li>Privilege Escalation</li>
    <li>Data Breaches</li>
</ul>

<h2>Lesson 12: Data Warehousing and Data Mining</h2>

<h3>Data Warehousing</h3>
<p>A data warehouse integrates data from multiple sources to support business decision-making.</p>
<ul>
    <li><strong>Characteristics:</strong> Subject-oriented, integrated, time-variant, non-volatile.</li>
    <li><strong>Architecture:</strong> Data sources → ETL → Warehouse → Data Marts → OLAP tools</li>
</ul>

<h3>Data Mining</h3>
<p>Extracting meaningful patterns and insights from large datasets.</p>
<ul>
    <li><strong>Techniques:</strong> Classification, clustering, association rule mining.</li>
    <li><strong>Applications:</strong> Market analysis, fraud detection, recommendation systems.</li>
</ul>

<h2>Reflections and Insights</h2>
<p>Lessons 9–12 have equipped me with vital knowledge of ensuring data reliability through transactions, securing data against breaches, and leveraging data for analytical purposes. These concepts solidify the foundational and practical aspects of database systems.</p>

<h2>Conclusion</h2>
<p>From understanding concurrency to exploring data warehousing, these lessons represent my evolution in database management and analytics. I now look forward to exploring real-time databases, distributed systems, and cloud-based storage in the future.</p>

</body>