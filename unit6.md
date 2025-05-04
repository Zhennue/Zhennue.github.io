---
layout: post
title: UNIT 6
image: assets/images/6.z.png
nav-menu: true
---

<!-- Main -->

<!-- Main -->

<head>
<meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indexing & Query Processing</title>
    <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
      padding: 20px;
      background-color: #1a1a1a;
      color: #eaeaea;
    }
    h1, h2, h3 {
      color: white;
    }
    section {
      margin-bottom: 2rem;
    }
    code {
      background: black;
      color: white;
      padding: 3px 5px;
      border-radius: 3px;
    }
    pre {
      background: black;
      color: white;
      padding: 10px;
      border-radius: 5px;
      overflow-x: auto;
    }
.concept {
      border-left: 4px solid #0ef;
      padding-left: 15px;
      margin-bottom: 1rem;
    }
    </style>
</head>
<body>

  <h1>Lesson 14 & 15: Indexing, Query Processing & Optimization</h1>

  <section>
    <h2>Indexing Overview</h2>
    <div class="concept">
      <p>- Indexes improve query performance by providing fast access paths to data.</p>
      <p>- Two types: <strong>Primary Index</strong> (based on ordering field) and <strong>Secondary Index</strong> (on non-ordering fields).</p>
    </div>
  </section>

<section>
    <h2>Types of Indexes</h2>
    <div class="concept">
      <p><strong>Dense Index:</strong> Index entry for every search key value.</p>
      <p><strong>Sparse Index:</strong> Index entries for only some values; assumes sorted data.</p>
      <p><strong>Multilevel Index:</strong> Index on top of another index to reduce size per level.</p>
      <p><strong>Clustered Index:</strong> Data is sorted according to the index; one per table.</p>
      <p><strong>Unclustered Index:</strong> Data is stored independently of the index order.</p>
    </div>
  </section>

  <section>
    <h2>B+ Trees</h2>
    <div class="concept">
      <p>- A self-balancing tree structure widely used in databases.</p>
      <p>- Leaf nodes contain actual data pointers; internal nodes store keys for navigation.</p>
      <p>- Efficient for range queries and dynamic inserts/deletes.</p>
    </div>
  </section>

  <section>
    <h2>Hash-Based Indexing</h2>
    <div class="concept">
      <p>- Uses a hash function to map search keys to locations.</p>
      <p>- Efficient for equality searches; not ideal for range queries.</p>
      <p><strong>Static Hashing:</strong> Fixed number of buckets.</p>
      <p><strong>Dynamic Hashing:</strong> Buckets split as data grows (e.g., Extendible Hashing).</p>
    </div>
  </section>
<section>
    <h2>Query Processing</h2>
    <div class="concept">
      <p>- Involves parsing SQL, translation to relational algebra, optimization, and execution.</p>
      <p>- Multiple plans can be generated for a single SQL query.</p>
    </div>
  </section>

  <section>
    <h2>Query Optimization</h2>
    <div class="concept">
      <p>- Goal: choose most efficient plan (in terms of time, I/O, memory).</p>
      <p>- Techniques include:</p>
      <ul>
        <li>Predicate Pushdown</li>
        <li>Join Ordering</li>
        <li>Use of Indexes</li>
        <li>Eliminating Redundant Operations</li>
      </ul>
    </div>
  </section>

<section>
    <h2>Cost-Based Optimization</h2>
    <div class="concept">
      <p>- Estimates cost using statistics like relation size, number of distinct values, etc.</p>
      <p>- Chooses plan with minimum estimated cost.</p>
      <p>- Considerations: number of disk accesses, CPU time, memory usage.</p>
    </div>
  </section>

  <section>
    <h2>Heuristic Optimization</h2>
    <div class="concept">
      <p>- Uses predefined transformation rules to reduce the search space of query plans.</p>
      <p>- Rules include:</p>
      <ul>
        <li>Perform selections early (push selections)</li>
        <li>Combine Cartesian products with selections into joins</li>
        <li>Use projections early to reduce tuple size</li>
      </ul>
    </div>
  </section>
<section>
    <h2>Example Query Plan</h2>
    <div class="concept">
      <p>SQL:</p>
      <pre><code>SELECT name FROM student WHERE age &gt; 20;</code></pre>
      <p>Query Plan:</p>
      <pre><code>π_name(σ_age&gt;20(Student))</code></pre>
    </div>
  </section>

</body>
</html>