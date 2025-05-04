---
layout: page
title: UNIT 5
image: assets/images/5.a.png
nav-menu: true
---

<!-- Main -->

<head>
<meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Database Normalization & Temporal Design</title>
    <style>
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

  </style>
</head>
<body>

  <h1>Database Normalization & Temporal Design</h1>

  <section>
    <h2>Good Relational Design Principles</h2>
    <div class="normal-form">
      <p>- Each relation corresponds to one entity or relationship.</p>
      <p>- Minimize nulls, avoid spurious tuples, prevent redundancy and modification anomalies.</p>
    </div>
  </section>

  <section>
    <h2>Functional Dependencies</h2>
    <div class="normal-form">
      <p>X → Y means attribute Y is functionally dependent on X.</p>
      <p>Armstrong's Axioms: Reflexivity, Augmentation, Transitivity.</p>
    </div>
  </section>

  <section>
    <h2>Normal Forms</h2>
    <div class="normal-form">
      <p><strong>1NF:</strong> Atomic values only.</p>
      <p><strong>2NF:</strong> Full functional dependency on the primary key.</p>
      <p><strong>3NF:</strong> No transitive dependencies.</p>
      <p><strong>BCNF:</strong> Determinant must be a candidate key.</p>
      <p><strong>4NF:</strong> No non-trivial multivalued dependencies except those on superkeys.</p>
      <p><strong>5NF (PJNF):</strong> Decompositions based on join dependencies.</p>
      <p><strong>DKNF:</strong> Based on domain and key constraints.</p>
    </div>
  </section>

  <section>
    <h2>Decomposition</h2>
    <div class="normal-form">
      <p>- Lossless join decomposition ensures no data loss.</p>
      <p>- Dependency preservation is ideal but sometimes sacrificed in BCNF.</p>
    </div>
  </section>

  <section>
    <h2>Atomic Domains</h2>
    <div class="normal-form">
      <p>- Each attribute should hold indivisible values.</p>
      <p>- Composite/multivalued attributes should be separated into different fields.</p>
    </div>
  </section>

  <section>
    <h2>Temporal Data Modeling</h2>
    <div class="normal-form">
      <p>- Time-bound data uses <code>start_date</code> and <code>end_date</code> columns.</p>
      <p>- Functional dependencies are time-relative. Primary keys must ensure valid time ranges.</p>
      <pre><code>course(course_id, title, dept_name, credits, start_date, end_date)</code></pre>
    </div>
  </section>

</body>
</html>