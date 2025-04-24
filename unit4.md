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
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
      padding: 20px;
      background-color: #1a1a1a;
      color: #eaeaea;
    }
    h1, h2, h3, h4 {
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
    .normal-form {
      border-left: 4px solid #0ef;
      padding-left: 15px;
      margin-bottom: 1rem;
    }
    footer {
      text-align: center;
      margin-top: 3rem;
      padding-top: 1rem;
      border-top: 1px solid #555;
      color: #aaa;
    }
  </style>
</head>
<body>

  <h1>Database Systems: Normalization Summary</h1>

  <section>
    <h2>First Normal Form (1NF)</h2>
    <div class="normal-form">
      <p>All attributes must contain only atomic (indivisible) values.</p>
      <p><strong>Example:</strong> Split <code>phone_numbers</code> into <code>phone1</code>, <code>phone2</code>, etc.</p>
    </div>
  </section>

  <section>
    <h2>Second Normal Form (2NF)</h2>
    <div class="normal-form">
      <p>No partial dependency on a candidate key. Fully functionally dependent.</p>
    </div>
  </section>

  <section>
    <h2>Third Normal Form (3NF)</h2>
    <div class="normal-form">
      <p>All non-key attributes are non-transitively dependent on the primary key.</p>
    </div>
  </section>

  <section>
    <h2>Boyce-Codd Normal Form (BCNF)</h2>
    <div class="normal-form">
      <p>Every determinant is a candidate key. Stricter than 3NF.</p>
    </div>
  </section>

  <section>
    <h2>Fourth Normal Form (4NF)</h2>
    <div class="normal-form">
      <p>No multivalued dependencies unless they're based on a candidate key.</p>
    </div>
  </section>

  <section>
    <h2>Modeling Temporal Data</h2>
    <div class="normal-form">
      <p>Track time-based data using <code>start_date</code> and <code>end_date</code> fields.</p>
      <pre><code>course(course_id, title, dept, credits, start_date, end_date)</code></pre>
    </div>
  </section>

  <footer>
    <p>© 2025 CST | Database Systems DBS101</p>
  </footer>

</body>
</html>