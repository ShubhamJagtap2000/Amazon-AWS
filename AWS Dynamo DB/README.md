**Source:**

[Video Link 1](https://youtu.be/k0fcbRj_pZE)

# What is DynamoDB?

- DynamoDB is a fully managed NoSQL Databse service offered by AWS
- It works on key-value pair and other data structure documents provided by Amazon

![Screenshot (208)](https://user-images.githubusercontent.com/63872951/118960930-674dbe00-b981-11eb-97b7-096f2fb58d4e.png)

# Fundamental Components of DynamoDB

**1. Attribute:** The simplest element in DynamoDB that stores data without any further division. It's like the fundamental element of this database solution.\
**2. Item:** Holds a set of attributes in a table. Set of attributes that can uniquely define your entry in a table. e.g. An item in Employee Records will identify asingle employee.\
**3. Table:** Holds a set of items. e.g. Employee Records will have Employee Name, Employee Id, Employee Addressand Phone number all will be stored in a table.

![Screenshot (209)](https://user-images.githubusercontent.com/63872951/118961917-76813b80-b982-11eb-9350-38038ce52d2d.png)

**4. Primary Key:** Unique attribute that is necessary while creating a table. It cannot be null at any given point. Hence, whilevinserting an item into the table, a primary key attribute is a must.

![Screenshot (211)](https://user-images.githubusercontent.com/63872951/118964049-b77a4f80-b984-11eb-83eb-91b679fbb8e8.png)

**5. Secondary Index:** Can be understood as the attribute that lets you query the data with or without the help of a Primary key. Following additional accesses can be achieved.

![Screenshot (212)](https://user-images.githubusercontent.com/63872951/118964670-5ef78200-b985-11eb-9a70-475b26dd8a24.png)

**6. DynamoDB Streams:** Additional.optional feature provided by DYnamoDB to keep a track of data modification events in a table. Here, each event is represented by a stream record.

![Screenshot (213)](https://user-images.githubusercontent.com/63872951/118965131-f4931180-b985-11eb-9f91-1ca1fba2e240.png)


# Why DynamoDB?
**Reasons why DYnamoDB is preffered**

![Screenshot (210)](https://user-images.githubusercontent.com/63872951/118962545-1c34aa80-b983-11eb-8d14-e577b7470a29.png)

