# MongoDB Notes

- What is MongoDB ?

  - MongoDB is an **open-source**, **document-oriented database** built on a **horizontal scalable architecture** that uses a **flexible schema** for storing large amounts of data with less relations.
    <br><br>

- MongoDB details:

  - **Open-source**
  - **Document-oriented** database
  - Storing large amounts of data
  - **Flexible data model** that allows to store unstructured data
  - Categorized as a NoSQL DB, because stores and retrieves data in collections and documents, instead of tables
  - Uses **BSON format** which is a binary style of JSON documents
  - Provides full indexing support, and replication with rich and intuitive APIs
    <br><br>

- What is BSON ?

  - **BSON - Binary JSON**, BSON's binary structure encodes type and length information, which allow it to be traversed much more quickly compared to JSON.
    <br><br>

- Advantages of MongoDB:

  - Schema migration is required for MongoDB, is a database without schemas.
  - Document queries are used because it is a document-oriented language, which is important for allowing dynamic queries.
  - In comparison to other relational databases, performance optimization is simple.
  - Due to the way it uses internal memory for data storage, it enables quick access to data.
  - Using sharding, MongoDB expands horizontally (partitioning data across various servers). Your data is separated and evenly placed across the shards. This helps the readers to easily find their data.
  - Easier to maintain than conventional databases
  - Replication of data and workload distributed have been employed to increase data availability and deliver high performance.
    <br><br>

- Disadvantages of MongoDB:

  - It does not support joins the way a relational database does. But join capability may be manually added to the page with the proper code. But it could cause execution to slow and impact performance.
  - MongoDB stores the key names of each value pair. Also, data redundancy occurs as a result of joins’ limitations. As a result, memory is seen more often than is required.
  - 16 MB is the maximum size limit for documents.
  - Document nesting is not possible for more than 100 levels.
    <br><br>

- Structural differences between MongoDB and MySql ?

  | MySql    | MongoDB    |
  | :------- | :--------- |
  | Database | Database   |
  | Table    | Collection |
  | Rows     | Documents  |

  <br>

- Different between MySql and MongoDB:

  1. **Data Structure:** Relational databases excel at managing structured data with fixed schemas, while MongoDB offers flexibility with its dynamic document model, allowing for easy data evolution.
  2. **Scalability:** Relational databases are vertically scalable, meaning you can increase server resources for improved performance. MongoDB, on the other hand, is horizontally scalable, enabling you to distribute data across multiple servers and handle large-scale applications.
  3. **Transactions:** Relational databases have robust support for complex transactions, ensuring data consistency and integrity. MongoDB supports atomic operations on a single document, but complex multi-document transactions are available only in recent versions.
  4. **Querying:** Relational databases use SQL for querying, which provides powerful relational algebra operations and join capabilities. MongoDB offers a flexible query language with a rich set of operators for working with document structures and embedded arrays.
  5. **Use Case Fit:** Consider your specific use case and requirements. Relational databases are typically a good choice for applications with structured data and strong relationships, while MongoDB shines when handling semi-structured or rapidly changing data.
     <br><br>

- MongoDB installation:

  - **MAC**

    - Prerequisites

      1. Make sure you have installed `"Homebrew"` with `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
      2. Install Xcode Command-Line Tools - `xcode-select --install`
      3. Download the official Homebrew formula for MongoDB and the Database Tools - `brew tap mongodb/brew`
      4. To update Homebrew and all existing formulae - `brew update`

    - Install Community Edition

      1. Install MongoDB - `brew install mongodb-community@7.0`
      2. To run MongoDB Community Edition as a macOS service - `brew services start mongodb-community@7.0`
      3. Stop all the existing running app - `brew services stop mongodb-community@7.0`

    - Verify that MongoDB is running

      1. If you started MongoDB as a macOS service - `brew services list`
      2. If you started MongoDB manually as a background process - `ps aux | grep -v grep | grep mongod`

    - for more information on Mac - https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/

    - Installation process for Ubuntu - https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-ubuntu/

    - Installation process for other version of Linux - https://www.mongodb.com/docs/manual/administration/install-on-linux/
      <br><br>

- Check existing Database: `show dbs`
- Used latest DB Database: `use latest_db`
- Insert document: `db.students.insertOne({ name: "Hello", age: 30 })`
- Find items: `db.students.find()`
- Update the data: `db.students.updateOne({ name: })`
