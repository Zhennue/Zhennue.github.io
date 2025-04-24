---
layout: post
title: UNIT 2
image: assets/images/6f.webp
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- Introduction -->
<section id="one">
            <div class="inner">
                <header class="major">
                    <h2>📌 ERD Quick Guide</h2>
                </header>
                <p><strong>"Turning data chaos into structured brilliance!"</strong></p>
            </div>
        </section>

<!-- Core Concepts -->
<section id="two" class="spotlights">
            <section>
                <a class="image">
                    <img src="Unit 2/3.jpg" alt="ERD Overview" />
                </a>
                <div class="content">
                    <div class="inner">
                        <header class="major">
                            <h3>What is an ERD?</h3>
                        </header>
                        <p>Entity Relationship Diagrams (ERDs) map the logical structure of a database. They help in designing systems by visualizing entities, attributes, and relationships.</p>
                    </div>
                </div>
            </section>
            
<section>
                <a class="image">
                </a>
                <div class="content">
                    <div class="inner">
                        <header class="major">
                            <h3>Entities & Attributes</h3>
                        </header>
                        <p>An <strong>Entity</strong> is a distinct object (e.g., Student, Book). Each entity has <strong>Attributes</strong>, which define its properties (e.g., Name, ID).</p>
                    </div>
                </div>
            </section>
            
<section>
                <a class="image">
                    <img src="Unit 2/3b.jpg" alt="Relationships Diagram" />
                </a>
                <div class="content">
                    <div class="inner">
                        <header class="major">
                            <h3>Relationships</h3>
                        </header>
                        <p>Relationships show how entities interact. Examples: <strong>One-to-One</strong> (Manager-Department), <strong>One-to-Many</strong> (Teacher-Students), <strong>Many-to-Many</strong> (Students-Courses).</p>
                    </div>
                </div>
            </section>
        </section>

<!-- Advanced Concepts -->
<section id="three" class="spotlights">
            <section>
                <a class="image">
                    <img src="Unit 2/3c.png" alt="Primary and Foreign Key" />
                </a>
                <div class="content">
                    <div class="inner">
                        <header class="major">
                            <h3>Keys & Identifiers</h3>
                        </header>
                        <p><strong>Primary Key:</strong> Uniquely identifies a record.<br>
                           <strong>Foreign Key:</strong> Links to a primary key in another entity.<br>
                           <strong>Super & Candidate Keys:</strong> Other potential unique identifiers.</p>
                    </div>
                </div>
            </section>
            
<section>
                <a class="image">
                    <img src="Unit 2/3d.jpg" alt="Cardinality Representation" />
                </a>
                <div class="content">
                    <div class="inner">
                        <header class="major">
                            <h3>Mapping Cardinalities</h3>
                        </header>
                        <p>Defines how many entities relate:<br>
                           <strong>1:1</strong> (Passport-Person), <strong>1:M</strong> (Department-Employees), <strong>M:M</strong> (Students-Courses).</p>
                    </div>
                </div>
            </section>
        </section>

<!-- Extended Features -->
<section id="four" class="spotlights">
            <section>
                <a class="image">
                    <img src="Unit 2/3e.png" alt="Extended ERD Features" />
                </a>
                <div class="content">
                    <div class="inner">
                        <header class="major">
                            <h3>Advanced ERD Concepts</h3>
                        </header>
                        <p><strong>Specialization:</strong> Subclasses of an entity (e.g., Employees → Manager & Staff).<br>
                           <strong>Generalization:</strong> Merging entities (e.g., Car & Bike → Vehicle).<br>
                           <strong>Aggregation:</strong> Higher-level relationships (e.g., Loan with Bank & Customer).</p>
                    </div>
                </div>
            </section>
        </section>

<!-- Conclusion -->
<section id="five">
            <div class="inner">
                <header class="major">
                    <h2>🚀 Quick Recap</h2>
                </header>
                <p>ERDs simplify database design by defining entities, relationships, and constraints.</p>
                <ul>
                    <li>✔️ <strong>Entities</strong>: Objects with attributes</li>
                    <li>✔️ <strong>Relationships</strong>: Define interactions</li>
                    <li>✔️ <strong>Keys</strong>: Maintain uniqueness</li>
                    <li>✔️ <strong>Cardinalities</strong>: Define entity associations</li>
                </ul>
            </div>
        </section>
    </div> <br><br>





<!-- Lesson - 4 -->

<!-- Main -->
<div id="main">

<!-- Introduction -->
<section id="one">
        <div class="inner">
            <header class="major">
                <h2>📌 Relational Model & Schema Design</h2>
            </header>
            <p><strong>"Structuring data for efficient storage and retrieval!"</strong></p>
        </div>
    </section>

<!-- Learning Outcomes -->
<section id="two" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>📖 Learning Outcomes</h3>
                    </header>
                    <ul>
                        <li>Understand relational data models 🏛️</li>
                        <li>Explain entity relationship diagrams 📊</li>
                        <li>Identify complex attributes 🧩</li>
                        <li>Determine primary keys & remove redundancy 🔑</li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- Core Concepts -->
<section id="three" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>📖 Relational Model</h3>
                    </header>
                    <p>A database structure that ensures:</p>
                    <ul>
                        <li><strong>Structure</strong>: Defines relations & contents 📋</li>
                        <li><strong>Integrity</strong>: Ensures data consistency ✅</li>
                        <li><strong>Manipulation</strong>: Provides query & update interfaces ⚙️</li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- Keys and Relations -->
<section id="four" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>🔑 Keys in Relational Model</h3>
                    </header>
                    <ul>
                        <li><strong>Primary Key</strong>: Uniquely identifies tuples 🎯</li>
                        <li><strong>Foreign Key</strong>: Maps attributes to another relation 🔄</li>
                        <li><strong>Superkey</strong>: Set of attributes uniquely identifying tuples 🔐</li>
                        <li><strong>Candidate Key</strong>: Potential primary keys 👀</li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- Example Tables -->
<section id="five" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>🔗 Example Relations</h3>
                    </header>
                    <h4>Student Table</h4>
                    <table>
                        <tr>
                            <th>StudentNo</th>
                            <th>CID</th>
                            <th>Name</th>
                            <th>Address</th>
                            <th>Programme_ID</th>
                        </tr>
                        <tr>
                            <td>12345</td>
                            <td>12827827223</td>
                            <td>Sonam</td>
                            <td>Thimphu</td>
                            <td>BESWE</td>
                        </tr>
                        <tr>
                            <td>24656</td>
                            <td>26735678768</td>
                            <td>Tandin Sonam</td>
                            <td>Bondey, Paro</td>
                            <td>BEIT</td>
                        </tr>
                    </table>

<h4>Programme Table</h4>
                    <table>
                        <tr>
                            <th>Programme_ID</th>
                            <th>Programme_Name</th>
                            <th>Start_Year</th>
                        </tr>
                        <tr>
                            <td>BESWE</td>
                            <td>B.E. in Software Eng.</td>
                            <td>2023</td>
                        </tr>
                        <tr>
                            <td>BEIT</td>
                            <td>B.E. in IT</td>
                            <td>2011</td>
                        </tr>
                    </table>
                </div>
            </div>
        </section>
    </section>

<!-- Schema Design -->
<section id="six">
        <div class="inner">
            <header class="major">
                <h3>📍 Schema Design</h3>
            </header>
            <p>Using ERD tools like <a href="https://erdplus.com/">ERDPlus</a> & enforcing constraints via <a href="https://www.geeksforgeeks.org/constraints-on-relational-database-model/">GeeksforGeeks</a> 🌐</p>
        </div>
    </section>

<!-- Conclusion -->
<section id="seven">
        <div class="inner">
            <header class="major">
                <h2>🚀 Quick Recap</h2>
            </header>
            <p>Relational models ensure structured, efficient database design.</p>
            <ul>
                <li>✔️ <strong>Entities</strong>: Objects with attributes</li>
                <li>✔️ <strong>Relationships</strong>: Define interactions</li>
                <li>✔️ <strong>Keys</strong>: Maintain uniqueness</li>
                <li>✔️ <strong>Schema Design</strong>: Organizes data efficiently</li>
            </ul>
        </div>
    </section>
</div> <br> <br>





<!-- Lesson-5 -->

<!-- Main -->
<div id="main">

<!-- Introduction -->
<section id="one">
        <div class="inner">
            <header class="major">
                <h2>📌 ERD to Relational Schema Translation</h2>
            </header>
            <p><strong>"Transforming entity relationships into structured databases!"</strong></p>
        </div>
    </section>

<!-- Space for Large Image -->
<section id="image-section">
             <div class="inner" style="text-align: center; margin: 20px 0;">
                <img src="Unit 2/5a.jpg" alt="Small Image 1" style="width: 40%; height: auto; border: 2px solid #ddd; padding: 10px;">
            </div>
            <div class="inner" style="text-align: center; margin: 20px 0;">
                <img src="Unit 2/5b.jpg" alt="Small Image 2" style="width: 40%; height: auto; border: 2px solid #ddd; padding: 10px;">
            </div>
    </section>

<!-- Core Concepts -->
<section id="two" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>📖 Introduction</h3>
                    </header>
                    <p>Both the E-R model and the relational database model are logical representations of real-world enterprises. Because they use similar design principles, we can convert an ER design into a relational schema.</p>
                    <p>Useful Resources:</p>
                    <ul>
                        <li><a href="https://palden518.github.io/DBS101.github.io/2024/02/20/unit2.html">Study Guide</a></li>
                        <li><a href="https://www.freecodecamp.org/news/crows-foot-notation-relationship-symbols-and-how-to-read-diagrams/">Crow’s Foot Notation</a></li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- ERD to Schema Steps -->
<section id="three" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>🔄 Converting ERD to Relational Schema</h3>
                    </header>
                    <ol>
                        <li>Create a table for each entity type.</li>
                        <li>Represent multivalued attributes in a separate table.</li>
                        <li>Use only sub-attributes for composite attributes.</li>
                        <li>Exclude derived attributes from tables.</li>
                        <li>Convert relationship sets into relations.</li>
                    </ol>
                </div>
            </div>
        </section>
    </section>

<!-- Mapping Relationships -->
<section id="four" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>🔗 Mapping Relationships</h3>
                    </header>
                    <p>Relationship sets are converted into relations by combining primary keys of participating entities.</p>
                    <ul>
                        <li><strong>1:1 Relationship:</strong> Foreign key is assigned to the entity with partial participation.</li>
                        <li><strong>1:N Relationship:</strong> The primary key of the "many" entity is used as a foreign key in the other.</li>
                        <li><strong>M:N Relationship:</strong> A new table is created with composite primary keys.</li>
                        <li><strong>Unary Relationships:</strong> Uses recursive foreign keys for 1:N or new tables for 1:M.</li>
                        <li><strong>Ternary Relationships:</strong> Requires a new table containing primary keys of all participating entities.</li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- Specialization & Generalization -->
<section id="five" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>📂 Specialization & Generalization</h3>
                    </header>
                    <p>Three ways to map specialization/generalization:</p>
                    <ul>
                        <li><strong>Method 1:</strong> Map each entity to its own table.</li>
                        <li><strong>Method 2:</strong> Only subclasses are mapped.</li>
                        <li><strong>Method 3:</strong> Only the superclass is mapped (may introduce NULL values).</li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- Conclusion -->
<section id="seven">
        <div class="inner">
            <header class="major">
                <h2>🚀 Quick Recap</h2>
            </header>
            <ul>
                <li>✔️ Convert ERD entities into tables</li>
                <li>✔️ Map relationships using primary & foreign keys</li>
                <li>✔️ Handle special cases like unary, ternary, and aggregation</li>
                <li>✔️ Use UML for broader software design</li>
            </ul>
        </div>
    </section>
</div> <br> <br>





<!-- Lesson-6 -->

<!-- Main -->
<div id="main">

<!-- Introduction -->
<section id="one">
        <div class="inner">
            <header class="major">
                <h2>📌 Relational Algebra</h2>
            </header>
            <p><strong>"Mastering the foundation of database queries!"</strong></p>
        </div>
    </section>

<!-- Space for Two Medium Images -->
<section id="two-images-section">
        <div class="inner" style="text-align: center; margin: 20px 0;">
            <img src="Unit 2/6c.jpg" alt="Small Image 2" style="width: 40%; height: auto; border: 2px solid #ddd; padding: 10px;">
        </div>
        <div class="inner" style="display: flex; justify-content: space-around; margin: 20px 0;">
            <div style="text-align: center;">
                <img src="Unit 2/6a.png" alt="Small Image 1" style="width: 40%; height: auto; border: 2px solid #ddd; padding: 10px;">
            </div>
            <div style="text-align: center;">
                <img src="Unit 2/6b.jpg" alt="Small Image 2" style="width: 40%; height: auto; border: 2px solid #ddd; padding: 10px;">
            </div>
        </div>
    </section>

<!-- Core Concepts -->
<section id="two" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>📖 Key Concepts</h3>
                    </header>
                    <ul>
                        <li>📌 <strong>Query Languages</strong>: Ways to request information from databases, including imperative, functional, and declarative approaches.</li>
                        <li>📌 <strong>Selection (σ)</strong>: Filters rows based on conditions.</li>
                        <li>📌 <strong>Projection (π)</strong>: Chooses specific columns.</li>
                        <li>📌 <strong>Union (∪)</strong>: Combines tuples from two relations.</li>
                        <li>📌 <strong>Intersection (∩)</strong>: Returns common tuples.</li>
                        <li>📌 <strong>Difference (-)</strong>: Finds tuples in one but not the other.</li>
                        <li>📌 <strong>Cartesian Product (×)</strong>: Merges all tuples from both relations.</li>
                        <li>📌 <strong>Join (⋈)</strong>: Merges tuples based on common attributes.</li>
                        <li>📌 <strong>Operands</strong>: Logical and comparison operators such as AND ( ∧ ), OR ( ∨ ), NOT (¬), Greater than (>), Less than (<), and Equal to (=).</li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- Extra Operations -->
<section id="three" class="spotlights">
        <section>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>✨ Extra Operations</h3>
                    </header>
                    <ul>
                        <li>🔹 <strong>Rename (ρ)</strong>: Changes attribute names.</li>
                        <li>🔹 <strong>Assignment (←)</strong>: Stores intermediate results.</li>
                        <li>🔹 <strong>Duplicate Elimination (δ)</strong>: Removes duplicates from results.</li>
                        <li>🔹 <strong>Aggregation (γ)</strong>: Computes summary statistics.</li>
                        <li>🔹 <strong>Sorting (τ)</strong>: Orders tuples based on attributes.</li>
                        <li>🔹 <strong>Division (÷)</strong>: Finds values related to all instances of another set.</li>
                    </ul>
                </div>
            </div>
        </section>
    </section>

<!-- Conclusion -->
<section id="seven">
        <div class="inner">
            <header class="major">
                <h2>🚀 Quick Recap</h2>
            </header>
            <ul>
                <li>✔️ Understand Relational Algebra operations.</li>
                <li>✔️ Learn query transformations.</li>
                <li>✔️ Bridge the gap between theory and SQL.</li>
                <li>✔️ Apply relational algebra for efficient query design.</li>
            </ul>
            <ul class="actions">
                    <li><a href="#" class="button next">Get Started</a></li>
            </ul>
        </div>
    </section>

</div>