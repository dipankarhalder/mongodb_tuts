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

- Structural differences between MongoDB and MySql ?

  | MySql    | MongoDB    |
  | :------- | :--------- |
  | Database | Database   |
  | Table    | Collection |
  | Rows     | Documents  |

  <br>

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

- Check existing Database: `show dbs`
- Used latest DB Database: `use latest_db`
- Insert document: `db.students.insertOne({ name: "Hello", age: 30 })`
- Find items: `db.students.find()`
- Update the data: `db.students.updateOne({ name: })`
