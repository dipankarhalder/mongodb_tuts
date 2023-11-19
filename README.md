# MongoDB Notes

- What is the meaning of Mongo ?

  The meaning of mongo is HUGE / HUMONGOUS, means It can store a large amount of data efficiently.

- What is MongoDB ?

  - MongoDB is an open-source document-oriented database that is used for storing large amounts of data with less relations.
  - It is categorized as a NoSQL (Not only SQL) database because it stores and retrieves data in collections and documents, instead of tables.
  - MongoDB uses BSON (document storage format) which is a binary style of JSON documents.
  - MongoDB has a flexible data model that allows you to store unstructured data.
  - It also provides full indexing support, and replication with rich and intuitive APIs.

- Differences structure between MongoDB and MySql ?

  | MySql    | MongoDB    |
  | :------- | :--------- |
  | Database | Database   |
  | Table    | Collection |
  | Rows     | Documents  |

- What is BSON ?

  - **BSON - Binary JSON**, BSON's binary structure encodes type and length information, which allow it to be traversed much more quickly compared to JSON.

- Installing MongoDB

  - **MAC -**

    - Follow the steps and run the commands one by one and make sure you have installed "Homebrew" on your MAC

      1. Install XCode `xcode-select --install`

      2. Download the official Homebrew formula for MongoDB `brew tap mongodb/brew`

      3. To update Homebrew and all existing formulae `brew update`

      4. Run the following command in your macOS Terminal application `brew install mongodb-community@7.0`

      5. Run or enable MongoDB on your local system `brew services start mongodb-community@7.0`

      6. Stop all the existing running app `brew services stop mongodb-community@7.0`

- Check existing Database: `show dbs`
- Used latest DB Database: `use latest_db`
- Insert document: `db.students.insertOne({ name: "Hello", age: 30 })`
- Find items: `db.students.find()`
- Update the data: `db.students.updateOne({ name: })`
