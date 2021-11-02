# Room
Overview about saving data with Room
We can save data in local database when the device cannot access the network by using Room.

Room benefits:
1. Compile-time verification of SQL queries.
2. Convenience annotations that minimize repetitive and error-prone boilerplate code.
3. Streamlined database migration paths.

## Primary components:
Major componenets in Room:
1. **The database class:** its purpose is for holds the database and serves as the main access point for the underlying connection to your app's persisted data.
2. **Data entities:** represent tables in your app's database.
3. **Data access objects (DAOs):** that provide methods that your app can use to query, update, insert, and delete data in the database.

 **To Create a table in Database We must use @Entity. Where the benefit of the room entity includes fields for each column.**

1. @PrimaryKey: Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table.
2. @ColumnInfo: To give the column a name.
3. @Ignore: It is used If an entity has fields that you don't want to persist.

We can have relationships in a room such as:
1. one-to-one relationships.
2. one-to-many relationships.
3. many-to-many relationships.

**Data Access Objects**: are used to access your application’s persisted data. They are a better and more modular way to access your database as compared to query builders or direct queries.

**A Data Access Objects can be either an interface or an abstract class.** If it’s an abstract class, it can optionally have a constructor that takes a RoomDatabase as its only parameter. Room creates each DAO implementation at compile time.

We can perform multiple operations using Data Access Objects :
Insertion @Insert
Updation @Update
Deletion @Delete
