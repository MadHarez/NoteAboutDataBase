## SQL简介
SQL（Structured Query Language，结构化查询语言）是一种用于管理和查询数据库的标准编程语言。它最初由IBM的唐纳德·D·张伯尔（Donald D. Chamberlin）和雷·F·博伊斯（Raymond F. Boyce）在1970年代中期开发。SQL的设计目标是提供一种统一的方法来访问和操作关系数据库管理系统（RDBMS）。 历史

1. 1974年： IBM的圣何塞实验室开始开发System R项目，这是第一个商业关系数据库系统。SQL作为这个项目的一部分被开发出来。
    
2. 1979年： SQL被正式命名为“SEQUEL”，后来为了避免与一个英国公司的商标冲突，改名为“SQL”。
    
3. 1986年： 美国国家标准协会（ANSI）发布了第一个SQL标准，称为SQL-86。
    
4. 1987年： 国际标准化组织（ISO）和ANSI发布了SQL-89标准，这是SQL的第一个国际标准。
    
5. 1992年： SQL-92发布，引入了更多的功能，如触发器、存储过程和面向对象的特性。
    
6. 1999年： SQL:1999（SQL3）发布，引入了更多的数据类型和XML支持。
    
7. 2003年： SQL:2003引入了更多的功能，如窗口函数和正则表达式。
    
8. 2006年： SQL:2006增加了对Unicode的支持。
    
9. 2011年： SQL:2011引入了对JSON的支持。
    
10. 2016年： SQL:2016进一步增强了JSON和XML的支持，并引入了更多的数据类型。 简介 SQL是一种声明式语言，它允许用户定义和查询数据，而不需要指定数据是如何被检索的。SQL的主要功能包括： • 数据查询： 使用SELECT语句从数据库中检索数据。 • 数据操作： 使用INSERT、UPDATE和DELETE语句来添加、修改和删除数据。 • 数据定义： 使用CREATE、ALTER和DROP语句来创建、修改和删除数据库对象（如表、视图、索引等）。 • 数据控制： 使用GRANT和REVOKE语句来控制数据库的访问权限。 SQL的语法和功能在不同的数据库系统中有所不同，但大多数数据库系统都遵循SQL标准，提供了SQL的某种形式的支持。常见的数据库系统包括MySQL、PostgreSQL、Oracle、SQL Server和SQLite等。 SQL的标准化和相关组织主要涉及以下几个方面：
    
11. 国际标准化组织（ISO）：ISO是一个独立的、非政府间的国际组织，其宗旨是制定和发布国际标准，为企业和消费者设立统一的基准。ISO成立于1947年，总部设在瑞士日内瓦，目前有165个成员。ISO标准覆盖了广泛的行业和领域，包括信息技术等。SQL的国际标准通常被认为是ISO/IEC 9075，该标准由多个部分组成，最新版本是2023版。
    
12. 美国国家标准委员会（ANSI）：ANSI是一个核准多种行业标准的组织。SQL作为关系型数据库所使用的标准语言，最初是基于IBM的实现在1986年被ANSI批准的。1987年，ISO把ANSI SQL作为国际标准。ANSI与ISO共同制定SQL标准，每个版本的标准都有一些增强和改进。
    
13. 中国：中国也是ISO标准委员会的成员国，积极参与标准的制定工作，并经常翻译一些国际标准对应的中文版。
    
14. ISO/IEC 9075：这是SQL的国际标准，由ISO和国际电工委员会（IEC）共同制定。ISO/IEC 9075由多个部分组成，最新版本是2023版，其中包括： • ISO/IEC 9075-1:2023：Framework (SQL/Framework)，介绍ISO/IEC 9075系列其他部分中使用的概念框架，用于指定SQL的语法以及SQL实现以该语言处理语句的结果，并定义了术语和符号。 • ISO/IEC 9075-2:2023：Foundation (SQL/Foundation)，定义了SQL数据的数据结构和基本操作，提供了用于创建、访问、维护、控制和保护SQL数据的功能。 这些组织和标准共同推动了SQL语言的发展和全球化应用，确保了不同数据库系统之间的兼容性和一致性。 SQL的有关标准主要包括以下几个部分，它们构成了ISO/IEC 9075系列标准：
    
15. ISO/IEC 9075-1: Framework (SQL/Framework) • 介绍ISO/IEC 9075系列其他部分中使用的概念框架，用于指定SQL的语法以及SQL实现以该语言处理语句的结果，并定义了术语和符号。
    
16. ISO/IEC 9075-2: Foundation (SQL/Foundation) • 定义了SQL数据的数据结构和基本操作，提供了用于创建、访问、维护、控制和保护SQL数据的功能。
    
17. ISO/IEC 9075-3: Call Level Interface (SQL/CLI) • 涉及SQL的调用级接口。
    
18. ISO/IEC 9075-4: Persistent Stored Modules (SQL/PSM) • 涉及持久存储模块，例如PL/SQL对于Oracle或T-SQL对于SQL Server。
    
19. ISO/IEC 9075-9: Management of External Data (SQL/MED) • 管理外部数据。
    
20. ISO/IEC 9075-10: Object Language Bindings (SQL/OLB) • 对象语言绑定。
    
21. ISO/IEC 9075-11: Information and Definition Schemas (SQL/Schemata) • 信息和定义模式。
    
22. ISO/IEC 9075-13: SQL Routines and Types Using the Java Programming Language (SQL/JRT) • 使用Java编程语言的SQL例程和类型。
    
23. ISO/IEC 9075-14: XML-Related Specifications (SQL/XML) • 涉及XML相关规范。
    
24. ISO/IEC 9075-15: Multi-dimensional arrays (SQL/MDA) • 多维数组，于2019年发布。 此外，还有一部分正在讨论中，可能成为未来的SQL标准的一部分： • ISO/IEC 9075-16: Property Graph Query (SQL/PGQ) • 属性图查询，正在为SQL:2020工作。 这些标准由ISO和IEC联合成立的技术委员会JTC1/SC32负责具体制定工作。SQL标准的符合性意味着一个SQL实现如果实现了所有强制性特性，则被称为符合标准的。SQL标准的各个部分涵盖了从基础的数据类型、DDL、DML、访问控制、事务控制到连接管理、会话管理、异常处理等多个方面。

### SQL的特点
1. **一体化：集DDL，DML，DCL于一体**
    
    - DDL（Data Definition Language）用于定义和管理数据库结构，如创建、修改和删除数据库、表、索引等。
    - DML（Data Manipulation Language）用于操作数据库中的数据，如插入、查询、更新和删除数据。
    - DCL（Data Control Language）用于定义数据访问和权限控制，如授权和撤销权限。
2. **单一的结构----关系，带来了数据操作符的统一**
    
    - SQL基于关系模型，数据以表格形式存储，每个表由行和列组成，这种结构的统一性使得数据操作和查询具有一致性。
3. **面向集合的操作方式：一次一集合**
    
    - SQL操作基于集合论，一次操作可以处理多个数据项，而不是单个数据项，这提高了数据处理的效率。
4. **高度非过程化：用户只需提出“做什么”，无须告诉“怎么做”**
    
    - SQL是非过程化的语言，用户只需要指定要执行的操作，而不需要编写具体的步骤来实现这些操作，数据库管理系统（DBMS）会负责执行细节。
5. **两种使用方式，统一的语法结构：SQL既是自含式语言（用户使用），又是嵌入式语言（程序员使用）**
    
    - SQL可以作为一个独立的语言直接在数据库管理系统中使用，也可以嵌入到其他编程语言中，如Java、C#等，以实现数据库操作。
6. **语言简洁，易学易用**
    
    - SQL的语法相对简单直观，易于学习和使用，使得非专业开发者也能快速上手。
7. **强大的查询能力**
    
    - SQL提供了丰富的查询功能，包括连接（JOIN）、子查询、分组（GROUP BY）、聚合函数（如COUNT、SUM、AVG等）和多种排序选项。
8. **事务控制**
    
    - SQL支持事务控制，确保数据的完整性和一致性。事务具有原子性、一致性、隔离性和持久性（ACID）特性。
9. **可移植性**
    
    - SQL标准定义了跨不同数据库系统的操作和查询的通用语法，提高了代码的可移植性。
10. **视图和存储过程**
    
    - SQL支持创建视图（View），它是一个虚拟表，可以简化复杂的查询操作。同时，存储过程（Stored Procedure）允许封装复杂的业务逻辑，提高代码的重用性和性能。
11. **数据完整性约束**
    
    - SQL支持多种数据完整性约束，如主键、外键、唯一性约束和检查约束，以确保数据的准确性和一致性。
12. **索引和优化**
    
    - SQL允许创建索引以提高查询性能，并提供了多种查询优化技术，以确保查询的高效执行。

这些特点共同构成了SQL的强大功能，使其成为数据库管理和操作的主流语言。


### SQL的基本概念
#### SQL支持的数据库三级模式
SQL支持的数据库三级模式与ANSI SPARC报告中的数据库三级模式在概念上是一致的，都是指外模式（External Schema）、概念模式（Conceptual Schema）和内模式（Internal Schema）。不过，它们在实现和支持方式上有所不同。以下是它们的对比和SQL对三级模式的支持：

1. **内部模式（Internal Schema）**
    
    - SQL通过表空间（Tablespace）、索引（Indexes）、分区（Partitioning）和存储过程（Stored Procedures）以及触发器（Triggers）来支持内部模式。这些特性允许数据库管理员定义数据的物理存储结构和访问方法，从而实现数据的物理独立性。
2. **概念模式（Conceptual Schema）**
    
    - SQL使用数据定义语言（DDL）如CREATE、ALTER、DROP语句来定义和修改数据库对象，包括表、视图、索引和约束等。同时，SQL通过完整性约束（如主键、外键、唯一性约束和检查约束）来保证数据的一致性和完整性，并使用外键来定义表之间的关系，维护数据的参照完整性。
3. **外部模式（External Schema）**
    
    - SQL通过视图（Views）为不同用户提供定制的数据视图，隐藏复杂的查询逻辑，提供简化的接口。此外，通过用户权限（User Permissions）和角色（Roles）管理用户对数据库对象的访问和操作，实现数据的用户独立性。

#### ANSI SPARC报告中的数据库三级模式

1. **外部模式（External Schema）**
    
    - ANSI SPARC体系结构中的外部模式是用户的数据视图，描述用户能够看见和使用的局部数据的逻辑结构和特征，与SQL中的外部模式相对应。
2. **概念模式（Conceptual Schema）**
    
    - 概念模式是数据库中全体数据的逻辑结构和特征的描述，是所有用户的公共数据视图，与SQL中的概念模式相对应。
3. **内部模式（Internal Schema）**
    
    - 内部模式描述数据的物理存储结构和存储方式，与SQL中的内部模式相对应。

#### 不同点

- **实现和使用**：SQL作为一种数据库查询和操作语言，提供了具体的语法和命令来实现三级模式的支持，而ANSI SPARC报告更多地定义了三级模式的概念和架构。
- **标准化程度**：ANSI SPARC体系结构是一个标准化的框架，而SQL的实现可能因不同的数据库管理系统（DBMS）而异，具有一定程度的灵活性和差异性。

总的来说，SQL在实现三级模式时提供了具体的语法和操作，而ANSI SPARC报告则定义了三级模式的理论框架。两者在概念上是一致的，但在实现细节上有所不同。

### SQL数据库体系结构
SQL数据库体系结构通常指的是关系型数据库管理系统（RDBMS）的架构，它遵循了数据库的三级模式结构，即外模式（External Schema）、概念模式（Conceptual Schema）和内模式（Internal Schema）。这种架构也被称为数据库的抽象层次结构，它允许不同级别的用户以不同的方式与数据库交互，同时保持数据的独立性和安全性。以下是SQL数据库体系结构的详细说明：

1. **外模式（External Schema）**
    
    - 外模式也被称为用户视图，是数据库用户能够看到的数据库的表示。它是数据库的一个子集，包含了用户感兴趣的数据和操作。外模式定义了用户与数据库交互的接口，用户通过外模式来访问和操作数据。
    - 在SQL中，外模式通常通过视图（Views）来实现，视图是一个虚拟表，它基于实际的表和/或其他视图，并且可以包含对这些表的复杂查询。
2. **概念模式（Conceptual Schema）**
    
    - 概念模式是数据库的整体逻辑结构，它描述了整个数据库的组织和结构，包括所有的表、视图、数据类型、约束和它们之间的关系。它是数据库的全局视图，为所有用户提供了一个统一的数据模型。
    - 在SQL中，概念模式通过数据定义语言（DDL）来定义，如CREATE TABLE、CREATE VIEW等语句。
3. **内模式（Internal Schema）**
    
    - 内模式也被称为存储模式，描述了数据在数据库内部的物理存储细节，包括数据的存储方式、索引、数据文件的组织结构等。
    - 在SQL中，内模式通常由数据库管理系统（DBMS）的存储引擎来管理，用户通常不需要直接与内模式交互。

除了三级模式结构，SQL数据库体系结构还包括以下几个关键组件：

4. **数据操纵语言（DML）**
    
    - DML包括INSERT、UPDATE、DELETE和SELECT语句，用于对数据库中的数据进行增删改查操作。
5. **数据控制语言（DCL）**
    
    - DCL包括GRANT和REVOKE语句，用于定义数据库的安全策略和访问权限。
6. **事务控制语言（TCL）**
    
    - TCL包括BEGIN TRANSACTION、COMMIT和ROLLBACK语句，用于管理数据库事务，确保数据的一致性和完整性。
7. **数据库缓冲区（Buffer Manager）**
    
    - 缓冲区管理器负责管理数据库数据在内存和磁盘之间的缓存，以提高数据访问效率。
8. **数据库事务日志（Transaction Log）**
    
    - 事务日志记录了所有对数据库进行的修改操作，用于恢复和保证事务的原子性和持久性。
9. **查询处理器（Query Processor）**
    
    - 查询处理器解析和优化SQL查询语句，并生成执行计划来执行查询。
10. **存储管理器（Storage Manager）**
    
    - 存储管理器负责管理数据库的物理存储，包括数据文件和索引文件的分配和释放。

SQL数据库体系结构的设计旨在提供一个灵活、可扩展和高效的数据管理环境，同时确保数据的安全性和一致性。

### SQL的分类
#### 数据定义语言（DDL） - Data Definition Language

DDL用于定义和管理数据库的结构，包括创建、修改和删除数据库对象。DDL语句通常由数据库管理员使用，以构建数据库的框架。
##### 1. **表（Tables）**：
   - **CREATE TABLE**：用于创建一个新表，并定义其结构，包括列名、数据类型和约束（如主键、外键、唯一性约束等）。
     ```sql
     CREATE TABLE table_name (
       column1 datatype constraint,
       column2 datatype constraint,
       ...
     );
     ```
   - **DROP TABLE**：用于删除一个已存在的表及其所有数据和结构。
     ```sql
     DROP TABLE table_name;
     ```
   - **ALTER TABLE**：用于修改已存在的表结构，如添加、删除或修改列，或者修改表的约束。
     ```sql
     ALTER TABLE table_name
     ADD column datatype;
     -- 或者
     ALTER TABLE table_name
     DROP COLUMN column;
     ```

##### 2. **视图（Views）**：
   - **CREATE VIEW**：用于创建一个视图，视图是一个虚拟表，其内容由查询定义。视图可以包含多个表和复杂的SQL操作。
     ```sql
     CREATE VIEW view_name AS
     SELECT column1, column2
     FROM table_name
     WHERE condition;
     ```
   - **DROP VIEW**：用于删除一个已存在的视图。
     ```sql
     DROP VIEW view_name;
     ```
   - **ALTER VIEW**：用于修改已存在的视图定义。
     ```sql
     ALTER VIEW view_name AS
     SELECT column1, column2
     FROM table_name
     WHERE condition;
     ```

##### 3. **索引（Indexes）**：
   - **CREATE INDEX**：用于创建一个索引，以提高查询性能。索引可以创建在表的一个或多个列上。
     ```sql
     CREATE INDEX index_name
     ON table_name (column);
     ```
   - **DROP INDEX**：用于删除一个已存在的索引。
     ```sql
     DROP INDEX index_name ON table_name;
     ```

DDL语句通常需要较高的权限，因为它们会改变数据库的结构。在执行DDL操作时，应该非常小心，因为这些操作可能会对数据库的性能和数据的完整性产生重大影响。在生产环境中，执行DDL操作之前，应该进行彻底的测试，并确保有数据备份和恢复计划。

- **CREATE**：用于创建新的数据库对象，如表、索引、视图、触发器等。
    
    ```sql
    CREATE TABLE Employees (
      ID int,
      Name varchar(100),
      Position varchar(100),
      Department varchar(100)
    );
    ```
    
- **ALTER**：用于修改现有数据库对象的结构，如添加或删除列。
    
    
    ```sql
    ALTER TABLE Employees
    ADD COLUMN Age int;
    ```
    
- **DROP**：用于删除数据库对象。
    
    
    ```sql
    DROP TABLE Employees;
    ```
    
- **TRUNCATE**：快速删除表中的所有行，但保留表结构。
    
    
    ```sql
    TRUNCATE TABLE Employees;
    ```
    
- **COMMENT**：为数据库对象添加注释。
    
    
    ```sql
    COMMENT ON TABLE Employees IS 'Employee table';
    ```
    

#### 数据操纵语言（DML） - Data Manipulation Language

DML用于对数据库中的数据进行查询和修改。

- **SELECT**：用于查询数据库中的数据。
    
    ```sql
    SELECT * FROM Employees;
    ```
    
- **INSERT**：用于向表中插入新的数据行。
    
    
    ```sql
    INSERT INTO Employees (ID, Name, Position, Department) VALUES (1, 'John Doe', 'Developer', 'IT');
    ```
    
- **UPDATE**：用于修改表中的现有数据。
    
    
    ```sql
    UPDATE Employees
    SET Position = 'Senior Developer'
    WHERE ID = 1;
    ```
    
- **DELETE**：用于从表中删除数据。
    
    sql
    
    ```sql
    DELETE FROM Employees
    WHERE ID = 1;
    ```
    

#### 数据控制语言（DCL） - Data Control Language

DCL用于控制数据库的安全和访问权限，定义用户对数据库对象的访问级别。

- **GRANT**：授予用户或角色对数据库对象的特定权限。
    
    
    ```sql
    GRANT SELECT, INSERT ON Employees TO 'user_name';
    ```
    
- **REVOKE**：撤销用户或角色对数据库对象的权限。
    
    
    ```sql
    REVOKE SELECT ON Employees FROM 'user_name';
    ```
    

#### 其他SQL类别

- **事务控制语言（TCL） - Transaction Control Language** 用于管理数据库事务，确保数据的完整性和一致性。
    
    - **BEGIN TRANSACTION** 或 **START TRANSACTION**：开始一个新的事务。
        
        
        ```sql
        BEGIN TRANSACTION;
        ```
        
    - **COMMIT**：提交事务，使所有更改永久生效。
        
        
        ```sql
        COMMIT;
        ```
        
    - **ROLLBACK**：回滚事务，撤销所有更改。
        
        
        ```sql
        ROLLBACK;
        ```
        
- **数据查询语言（DQL） - Data Query Language** 通常被视为DML的一部分，但有时单独列出，专门用于查询数据。
    
    - **SELECT**：查询数据库中的数据。

这些类别共同构成了SQL语言的基础，使得用户能够全面地管理和操作数据库。


### SQL语句中的9个核心动词
你总结得非常准确，SQL（Structured Query Language）是一种用于管理和操作关系数据库的强大语言。下面是你提到的9个核心动词的简要说明：

1. **SELECT**：用于查询数据库中的数据，可以指定查询哪些列或使用星号（*）来选择所有列。
	- 用于查询数据库中的数据。
	- 可以结合`WHERE`子句进行条件查询。
	- 可以与`ORDER BY`子句一起使用，对结果进行排序。
	- 可以与`GROUP BY`子句一起使用，进行分组统计。
	- 例子：`SELECT column1, column2 FROM table_name WHERE condition;`

2. **CREATE**：用于创建新的数据库对象，如表、视图、索引、触发器等。
	- 创建新的数据库对象。
	- 可以创建表、数据库、索引、视图、触发器等。
	- 例子：`CREATE TABLE table_name (column1 datatype, column2 datatype, ...);`

3. **ALTER**：用于修改已存在的数据库对象的结构，如添加或删除列。
	- 修改已存在的数据库对象的结构。
	- 可以添加、删除或修改表中的列。
	- 例子：`ALTER TABLE table_name ADD column datatype;`

4. **DROP**：用于删除数据库对象，如表、视图、索引等。
	- 修改已存在的数据库对象的结构。
	- 可以添加、删除或修改表中的列。
	- 例子：`ALTER TABLE table_name ADD column datatype;`
5. **INSERT**：用于向表中插入新的数据行。
	- 向表中插入新的数据行。
	- 可以插入单行或多行数据。
	- 例子：`INSERT INTO table_name (column1, column2) VALUES (value1, value2);`
6. **UPDATE**：用于修改表中的现有数据。
	- 修改表中的现有数据。
	- 可以结合`WHERE`子句指定更新条件。
	- 例子：`UPDATE table_name SET column1 = value1 WHERE condition;`
7. **DELETE**：用于从表中删除数据。
	- 从表中删除数据。
	- 可以结合`WHERE`子句指定删除条件。
	- 例子：`DELETE FROM table_name WHERE condition;`
8. **GRANT**：用于授予用户或角色对数据库对象的特定权限。
	- 授予用户或角色对数据库对象的特定权限。
	- 可以授予的权限包括SELECT、INSERT、UPDATE、DELETE等。
	- 例子：`GRANT SELECT, INSERT ON table_name TO user_name;`
9. **REVOKE**：用于撤销之前授予用户或角色的权限。
	- 撤销之前授予用户或角色的权限。
	- 可以撤销单个权限或多个权限。
	- 例子：`REVOKE SELECT ON table_name FROM user_name;`
这些动词构成了SQL语言的基础，使得用户能够执行各种数据库操作。

## 基本的数据定义
在SQL中，对于基本表的创建、修改和删除，你可以使用以下核心动词和相应的SQL语句：

### 1. **创建基本表（CREATE TABLE）**：
   - 用于创建一个新的表。
   - 你需要指定表名和列的定义，包括数据类型和其他约束（如主键、外键、索引等）。
   - 例子：
     ```sql
     CREATE TABLE Employees (
         EmployeeID int NOT NULL,
         FirstName varchar(255) NOT NULL,
         LastName varchar(255) NOT NULL,
         BirthDate datetime NULL,
         HireDate datetime NULL,
         Position varchar(255) NULL,
         DepartmentID int NULL,
         PRIMARY KEY (EmployeeID)
     );
     ```

### 2. **表结构的修改（ALTER TABLE）**：
   - 用于修改已存在的表结构。
   - 可以添加、删除或修改列，也可以修改表的约束。
   - 例子：
     - 添加列：
       ```sql
       ALTER TABLE Employees
       ADD MiddleName varchar(255) NULL;
       ```
     - 删除列：
       ```sql
       ALTER TABLE Employees
       DROP COLUMN MiddleName;
       ```
     - 修改列的数据类型：
       ```sql
       ALTER TABLE Employees
       ALTER COLUMN Position varchar(500);
       ```

### 3. **删除基本表（DROP TABLE）**：
   - 用于删除一个已存在的表。
   - 一旦执行，表及其所有数据和结构将被永久删除。
   - 例子：
     ```sql
     DROP TABLE Employees;
     ```
   - **警告**：使用`DROP TABLE`时要非常小心，因为这会永久删除表和数据。在执行之前，确保备份了所有重要数据。
### 数据类型

1. **字符型**：
   - **Char(n)**：固定长度的字符串数据类型，`n`表示字符长度。如果存储的字符串短于`n`，剩余的位置会用空格填充。
     - 例如：`Char(5)`会存储最多5个字符的字符串，如`'Kimi '`（末尾有三个空格）。
   - **Varchar(n)**：可变长度的字符串数据类型，`n`表示最大字符长度。实际存储时，只占用必要的空间加上一个额外字节来记录长度。
     - 例如：`Varchar(255)`可以存储最多255个字符的字符串。

2. **数值型**：
   - **整数型**：
     - **bigint**：8字节整数，范围从-2^63到2^63-1。
     - **int**：4字节整数，范围从-2^31到2^31-1。
     - **smallint**：2字节整数，范围从-2^15到2^15-1。
     - **tinyint**：1字节整数，范围从0到255。
   - **小数型**：
     - **numeric** 和 **decimal**：用于存储精确的小数。它们可以指定精度（总位数）和小数位数。
       - 例如：`numeric(10, 2)`或`decimal(10, 2)`表示总共10位数字，其中2位是小数。

3. **货币型**：
   - **money**：用于存储货币值，精度为小数点后4位，范围从-922,337,203,685,477.5808到922,337,203,685,477.5807。
   - **smallmoney**：用于存储较小的货币值，精度为小数点后4位，范围从-214,748.3648到214,748.3647。

4. **日期型**：
   - **datetime**：用于存储日期和时间，范围从1753-01-01 00:00:00到9999-12-31 23:59:59.997。
   - **smalldatetime**：用于存储日期和时间，但精度较低，只精确到分钟，范围从1900-01-01 00:00:00到2079-06-06 23:59:59。

5. **文本型**：
   - **text**：用于存储大量文本数据，最大长度为2^16-2（约65534）字符。

6. **逻辑型**：
   - **bit**：用于存储布尔值，只有0（假）和1（真）两个值。

选择合适的数据类型对于数据库性能和存储效率至关重要。例如，使用`varchar`而不是`char`可以节省空间，因为`varchar`只存储必要的字符长度。同样，选择合适的数值类型可以确保数据的准确性和存储效率。



### 数据库的建立与撤销

1. **建立一个新数据库**
   - 命令：`CREATE DATABASE 数据库名`
   - 这个命令用于创建一个新的数据库。你需要提供数据库的名称作为参数。

2. **撤销一个数据库**
   - 命令：`DROP DATABASE 数据库名`
   - 这个命令用于删除一个已经存在的数据库。你需要提供要删除的数据库名称作为参数。注意，这个操作会删除数据库及其所有内容，所以请谨慎使用。

3. **指定当前数据库**
   - 命令：`USE 数据库名`
   - 这个命令用于指定当前的数据库上下文。在执行数据库操作之前，你需要确保你正在操作的是正确的数据库。

#### 创建grademanager数据库

以下是创建名为`grademanager`的数据库的具体SQL语句：

```sql
CREATE DATABASE grademanager
ON 
(NAME=grademanager_data, 
 FILENAME='C:\MSSQL7\data\grademanager_Data.MDF', 
 SIZE=10, 
 FILEGROWTH=10%)
LOG ON 
(NAME=grademanager_log, 
 FILENAME='C:\MSSQL7\data\grademanager_log.LDF',
 SIZE=5,
 FILEGROWTH=10%)
```

- **解释**：
  - `CREATE DATABASE grademanager`：创建一个名为`grademanager`的新数据库。
  - `ON (NAME=grademanager_data, FILENAME='C:\MSSQL7\data\grademanager_Data.MDF', SIZE=10, FILEGROWTH=10%)`：指定数据库的数据文件（MDF）的逻辑名称、物理路径、初始大小和增长设置。
    - `NAME=grademanager_data`：数据文件的逻辑名称。
    - `FILENAME='C:\MSSQL7\data\grademanager_Data.MDF'`：数据文件的物理路径。
    - `SIZE=10`：数据文件的初始大小为10MB。
    - `FILEGROWTH=10%`：数据文件的增长设置为每次增长10%。
  - `LOG ON (NAME=grademanager_log, FILENAME='C:\MSSQL7\data\grademanager_log.LDF', SIZE=5, FILEGROWTH=10%)`：指定数据库的日志文件（LDF）的逻辑名称、物理路径、初始大小和增长设置。
    - `NAME=grademanager_log`：日志文件的逻辑名称。
    - `FILENAME='C:\MSSQL7\data\grademanager_log.LDF'`：日志文件的物理路径。
    - `SIZE=5`：日志文件的初始大小为5MB。
    - `FILEGROWTH=10%`：日志文件的增长设置为每次增长10%。

这个SQL语句提供了创建数据库时对数据文件和日志文件的详细配置，确保数据库的存储和日志记录按照预期进行。


#### 创建表

```sql
CREATE TABLE <表名>
(<列名> <数据类型> [NULL | NOT NULL], …,
[PRIMARY KEY <关键字>,]
[FOREIGN KEY <外来关键字> REFERENCES <外来关键字所属表名>, …,]
[CHECK <校验条件>,]);
```

#### 删除表


```sql
DROP TABLE <表名1>[，<表名2>] 
```

#### 修改表结构


```sql
ALTER TABLE <表名>
[ ADD <列名><数据类型>[列的完整性约束]]| [ ADD <表级完整性约束>]
[ ALTER COLUMN <列名><新的数据类型>] 
[ DROP COLUMN <列名>] 
[ DROP CONSTRAINT <表级完整性约束名>];
```



### 索引
#### 索引的概念和作用

**概念**： 索引是数据库表中一列或多列的值存储的数据结构，它允许数据库系统快速检索、更新、删除或插入表中的数据。索引类似于书籍的目录，可以帮助快速定位到数据的位置，而不需要扫描整个表。

**作用**：

- **提高查询速度**：索引可以显著减少查询中需要扫描的数据量，从而加快查询速度。
- **加速表与表之间的连接**：如果两个表有共同的列，并且这些列上有索引，那么连接操作可以更快完成。
- **维护数据的唯一性**：唯一性索引可以保证列中的值是唯一的。

#### 索引的类型

##### 1. **聚簇索引（Clustered Index）**：
    
    - 表中数据的物理存储顺序与索引键值的顺序相同。
    - 一个表只能有一个聚簇索引。
    - 聚簇索引通常用于主键。
##### 2. **非聚簇索引（Nonclustered Index）**：
    
    - 表中数据的物理存储顺序与索引键值的顺序无关。
    - 一个表可以有多个非聚簇索引。
    - 非聚簇索引类似于书的目录，指向数据的实际位置。
##### 3. **唯一性索引（Unique Index）**：
    
    - 保证索引列中的值是唯一的。
    - 可以是聚簇的也可以是非聚簇的。
##### 4. **非唯一性索引（Non-unique Index）**：
    
    - 不保证索引列中的值是唯一的。

#### 如何使用企业管理器创建和管理索引

在SQL Server Management Studio (SSMS) 中，你可以通过图形界面来创建和管理索引：

- 右键点击表，选择“索引”。
- 在弹出的窗口中，你可以添加新的索引或修改现有的索引。
- 指定索引的类型（聚簇或非聚簇）、列和排序顺序。

#### 如何使用T-SQL语句创建和管理索引

**创建索引**：


```sql
CREATE [UNIQUE] [CLUSTERED | NONCLUSTERED] INDEX index_name
ON table_name (column_name [ASC | DESC], ...);
```

**删除索引**：


```sql
DROP INDEX index_name ON table_name;
```

#### 索引的作用

- **提高查询效率**：如你所述，索引可以显著提高查询条件中包含的列的查询速度。

#### 索引使用的场所

- **限制**：创建索引需要时间和存储空间，并且可能会降低数据插入、更新和删除的速度，因为索引本身也需要被更新。
- **平衡**：需要在查询性能和数据修改性能之间找到平衡点。

#### 索引的创建和删除示例

**创建聚簇索引**：（Only For SQL Server)


```sql
CREATE CLUSTERED INDEX idx_column ON table_name (column_name);
```

**创建非聚簇索引**：Only For SQL Server)


```sql
CREATE NONCLUSTERED INDEX idx_column ON table_name (column_name);
```

**删除索引**：


```sql
drop index [index_name] (on [table_name]) index_name
```

注意！索引在`MySQL、SQL Server`中非全局唯一，因此需要置顶`on table_name.`
而在`Pg，Oracle`中全局唯一，因此不需要指定`On Table_Name`

### 数据查询

**含义**：
查询是从数据库中检索数据的过程。在关系数据库中，这是通过SQL（Structured Query Language）来完成的。

#### SELECT语句

**最基本形式**：
```sql
SELECT column1, column2
FROM table_name;
```
这将从`table_name`表中选择`column1`和`column2`列的所有数据。

**完整语法**：
```sql
SELECT [DISTINCT | ALL] column1, column2
FROM table_source
[WHERE condition]
[GROUP BY group_by_expression]
[HAVING condition]
[ORDER BY order_expression [ASC | DESC]];
```
- `DISTINCT`关键字用于返回唯一不同的值。
- `ALL`关键字（默认）返回所有值，包括重复的。
- `WHERE`子句用于过滤结果集。
- `GROUP BY`用于将结果集按一个或多个列的值进行分组。
- `HAVING`子句用于对分组后的结果进行条件过滤。
- `ORDER BY`用于对结果集进行排序。

#### 检索数据

**查询表中列**：
```sql
SELECT * FROM table_name;
```
这将选择`table_name`表中的所有列。

**查询关系中所有信息**：
```sql
SELECT * FROM table_name1, table_name2;
```
这将执行两个表的笛卡尔积，返回所有可能的行组合。

#### 条件选择查询

```sql
SELECT column1, column2
FROM table_name
WHERE column1 = 'value';
```
这将选择`table_name`表中`column1`等于'value'的所有行。

#### 查询结果排序

```sql
SELECT column1, column2
FROM table_name
ORDER BY column1 ASC, column2 DESC;
```
这将按`column1`升序和`column2`降序排序结果。

#### 聚合函数

聚合函数对一组值执行计算，并返回单个值。

```sql
-- 计算行数
SELECT COUNT(*) FROM table_name;

-- 计算特定列的不同值的数量
SELECT COUNT(DISTINCT column_name) FROM table_name;

-- 计算特定列的最大值
SELECT MAX(column_name) FROM table_name;

-- 计算特定列的最小值
SELECT MIN(column_name) FROM table_name;

-- 计算特定列的总和
SELECT SUM(column_name) FROM table_name;

-- 计算特定列的平均值
SELECT AVG(column_name) FROM table_name;
```

#### 数据分组

```sql
SELECT column_name, COUNT(*)
FROM table_name
GROUP BY column_name;
```
这将按`column_name`的值对结果进行分组，并计算每个组的行数。

#### HAVING

```sql
SELECT column_name, COUNT(*)
FROM table_name
GROUP BY column_name
HAVING COUNT(*) > 1;
```
这将返回`column_name`组中行数大于1的组。

#### 表连接

**广义笛卡尔积（交叉连接）**：
```sql
SELECT a.*, b.*
FROM table_a a
CROSS JOIN table_b b;
```
这将返回`table_a`和`table_b`的所有可能组合。

**等值连接（含自然连接）**：
```sql
SELECT a.column_name, b.column_name
FROM table_a a
INNER JOIN table_b b ON a.common_column = b.common_column;
```
这将基于`common_column`列的相等值连接`table_a`和`table_b`。

**自然连接**：
```sql
SELECT a.*, b.*
FROM table_a
NATURAL JOIN table_b;
```
这将自动匹配两个表中同名的列，并基于这些列的相等值进行连接。

**非等值连接**：
```sql
SELECT a.column_name, b.column_name
FROM table_a a
LEFT JOIN table_b b ON a.common_column <> b.common_column;
```
这将基于`common_column`列的不相等值连接`table_a`和`table_b`。

通过这些详细的说明，你应该能够更好地理解SQL查询的各个方面，以及如何使用它们来从数据库中检索和操作数据。

#### 自身连接查询

自身连接查询是指一个表与自身进行连接查询。这通常发生在需要比较表中不同行的数据时。

```sql
SELECT a.*, b.*
FROM table_name a, table_name b
WHERE a.id = b.parent_id;
```

在这个例子中，`table_name`与自身进行连接，通过`id`和`parent_id`字段将不同的行连接起来。

#### 外连接查询

外连接查询可以返回两个表中的所有行，即使在连接条件中没有匹配的行也会返回。外连接分为左外连接、右外连接和全外连接。

##### - **左外连接**：


```sql
SELECT a.*, b.*
FROM table_a a
LEFT OUTER JOIN table_b b ON a.id = b.a_id;
```

这将返回`table_a`中的所有行，以及`table_b`中匹配`a.id`和`b.a_id`的行。如果`table_b`中没有匹配的行，则`b.*`的结果为NULL。

##### - **右外连接**：

```sql
SELECT a.*, b.*
FROM table_a a
RIGHT OUTER JOIN table_b b ON a.id = b.a_id;
```

这将返回`table_b`中的所有行，以及`table_a`中匹配`a.id`和`b.a_id`的行。如果`table_a`中没有匹配的行，则`a.*`的结果为NULL。

##### - **全外连接**（在某些数据库系统中可能不支持）：


```sql
SELECT a.*, b.*
FROM table_a a
FULL OUTER JOIN table_b b ON a.id = b.a_id;
```

这将返回两个表中的所有行，无论它们是否匹配。

#### 复合条件连接查询

复合条件连接查询是指在`JOIN`子句中使用多个条件来连接表。

```sql
SELECT a.*, b.*
FROM table_a a
JOIN table_b b ON a.id = b.a_id AND a.status = b.status;
```

在这个例子中，`table_a`和`table_b`不仅通过`id`连接，还需要`status`字段匹配。

#### 集合运算

集合运算允许对两个查询结果集进行并、交、差等操作。

##### - **并操作（UNION）**：



```sql
SELECT column_name FROM table1
UNION
SELECT column_name FROM table2;
```

`UNION`操作符用于合并两个查询结果集，自动去除重复行。

##### - **交操作（INTERSECT）**：


```sql
SELECT column_name FROM table1
INTERSECT
SELECT column_name FROM table2;
```

`INTERSECT`操作符返回两个查询结果集的交集。

##### - **差操作（EXCEPT或MINUS）**：



```sql
SELECT column_name FROM table1
EXCEPT
SELECT column_name FROM table2;
```

`EXCEPT`操作符返回存在于第一个查询结果集中但不在第二个查询结果集中的行。在某些数据库系统中，可能使用`MINUS`关键字。

#### 子查询

子查询是嵌套在另一个查询中的SQL查询。

##### - **嵌套子查询**：



```sql
SELECT * FROM customers
WHERE customer_id IN (SELECT customer_id FROM orders);
```

这个查询将返回所有在`orders`表中有订单的客户。

##### - **相关子查询**：
- 相关子查询是指子查询中的查询依赖于包含它的外部查询。

```sql
SELECT * FROM employees e1
WHERE e1.salary > (SELECT AVG(salary) FROM employees e2 WHERE e2.department = e1.department);
```

这个查询将返回薪水高于其所在部门平均薪水的所有员工。

### 视图
视图（View）是数据库中的一个重要概念，它是一个虚拟表，其内容由查询定义。视图可以包含多个表和复杂的SQL操作，但它本身不存储数据，而是在查询时动态生成数据。以下是视图的一些补充说明：

#### 视图的优点

1. **逻辑数据独立性**：
    
    - 视图可以隐藏底层表结构的复杂性，用户不需要知道数据是如何存储的，只需要通过视图来访问数据。
2. **简化和自定义数据访问**：
    
    - 用户可以通过视图来定制他们需要的数据，使得数据访问更加直观和方便。
3. **数据安全保护**：
    
    - 通过视图，可以限制用户直接访问基表，只允许他们访问视图中定义的数据，从而保护数据的安全。

#### 创建视图

```sql
CREATE VIEW view_name AS
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

- `WITH ENCRYPTION`：指定视图的定义不能被查看，但可以被使用。
- `WITH CHECK OPTION`：确保对视图进行的INSERT、UPDATE和DELETE操作满足视图的定义条件。

#### 管理视图

- **显示视图信息**：
    
    
    ```sql
    EXEC sp_help 'view_name';
    ```
    
    这将显示视图的名称、拥有者、创建时间等信息。
    
- **显示视图定义**：
    
    
    ```sql
    EXEC sp_helptext 'view_name';
    ```
    
    这将显示视图的定义语句。
    
- **查看视图依赖关系**：
    
    
    ```sql
    EXEC sp_depends 'view_name';
    ```
    
    这将查看视图与其他数据库对象之间的依赖关系。
    

#### 修改视图



```sql
ALTER VIEW view_name AS
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

使用`ALTER VIEW`语句可以修改视图的定义。

#### 删除视图



```sql
DROP VIEW view_name;
```

使用`DROP VIEW`语句可以删除视图。

#### 通过视图修改基表中数据

- **查询**：
    
    
    ```sql
    SELECT * FROM view_name;
    ```
    
    这将查询视图，并返回基表中的数据。
    
- **插入**：
    
    
    ```sql
    INSERT INTO view_name (column1, column2) VALUES (value1, value2);
    ```
    
    这将向基表中插入数据。
    
- **更新**：
    
    
    ```sql
    UPDATE view_name SET column1 = value1 WHERE condition;
    ```
    
    这将更新基表中的数据。
    
- **删除**：
    
    
    ```sql
    DELETE FROM view_name WHERE condition;
    ```
    
    这将从基表中删除数据。
    

#### 注意事项

- 视图可以简化复杂的SQL操作，使得用户可以像操作普通表一样操作视图。
- 视图可以提高数据的安全性，通过限制对基表的直接访问。
- 视图的修改（如插入、更新、删除）会直接影响基表中的数据，因此在使用视图进行数据操作时需要谨慎。
- 视图的定义可以包含复杂的SQL逻辑，如连接（JOIN）多个表、使用聚合函数等。