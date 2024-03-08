# Day 14 Notes:
- The rule is to do small commits and commit often.
- git init -> for new projects so that git can track it
- black disks are less prone to vibrations and higher life -> more expensive
- Server erorr -> When the server receives more requests than it can handle.
    - To handle this you can add more ram (Vertical -> making PC more powerful) or add more servers/PCs (Horizontal)
- Auto-scaling -> as the load increases auto-scaling will add/rent more PCs for you -> Pay as you go model. 
- DevOps -> Mantain aws
- DDOS -> Distributed Denail of Service -> Keeping the website busy
    - Prevent it by redirecting the bots -> ask "are you a bot"
- Features od DBs:
    - Use of cache/ram
    - Querying becomes easier
    - CRUD - easy
    - Backups are inbuilt
    - Undo - easisly (time limit)
- NoSQL -> Real time database
- SQL -> PostgreSQL


## SQL
- Structures Query Language -> a language designed to allow technical and non-technical users to work with databses.
- `==` is case-sensitive and `LIKE` matches anything closer:
- `%` acts like `.*` (any character 0 or more times) -> Matches anything
- `_` -> exactly one (no more no less)
- Anomalies -> Data mismatch
- First Normal Form Rules:
    - Should not use row order to convey information
    - Do not mix data types in each column
    - Table should have a primary key.
    - repeating groups are not allowed
- Second Normal form:
    - Every column in the table should depend on the primary key.
    - The second Normal Form (2NF) is based on the concept of fully functional dependency. The second Normal Form applies to relations with composite keys, that is, relations with a primary key composed of two or more attributes
    - every non-primary-key attribute is fully functionally dependent on the primary key, then the relation is in Second Normal Form (2NF).
- Third Normal Form:
    - Every non-key attribute in a table should depend on the key, the whole key, and nothing but the key.
- Primary key:
    - Unique
    - Not null
    - Only one in a table

### JOINS
- Inner Join -> Intersection
- Outer Join:
    - Left Join -> Same results as inner join plus extra rows from table A
    - Right Join -> Same results as inner join plus extra rows from table B
    - Full Join -> Results from all tables combined
    




