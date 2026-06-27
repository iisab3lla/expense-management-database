<div align="center">

# Business Expense Management System

### Web Application with Relational Database Modeling

A web application for managing business expenses, focused on database modeling, CRUD operations, PHP and MySQL integration, and data persistence through a relational database.

</div>

<div align="center">

![PHP](https://img.shields.io/badge/PHP-Backend-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Relational%20Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![XAMPP](https://img.shields.io/badge/XAMPP-Local%20Environment-FB7A24?style=for-the-badge&logo=xampp&logoColor=white)
![PDO](https://img.shields.io/badge/PDO-Database%20Connection-374151?style=for-the-badge)
![InfinityFree](https://img.shields.io/badge/InfinityFree-Deployment-2563EB?style=for-the-badge)

</div>

---

## Project Snapshot

<table> 
  <tr>
    <td><strong>Project Type</strong></td>
    <td>Web application with relational database integration</td>
  </tr>
  <tr>
    <td><strong>Main Goal</strong></td>
    <td>Register, organize and persist business expense data in a MySQL database</td>
  </tr>
  <tr>
    <td><strong>Main Focus</strong></td>
    <td>Database modeling, table relationships, CRUD operations and PHP-MySQL integration</td>
  </tr>
  <tr>
    <td><strong>Backend</strong></td>
    <td>PHP with PDO</td>
  </tr>
  <tr>
    <td><strong>Database</strong></td>
    <td>MySQL</td>
  </tr>
  <tr>
    <td><strong>Local Environment</strong></td>
    <td>XAMPP with Apache and MySQL</td>
  </tr>
  <tr>
    <td><strong>Deployment</strong></td>
    <td>InfinityFree</td>
  </tr>
</table>

---

## Navigation

<table>
  <tr>
    <td><a href="#overview"><strong>Overview</strong></a><br>What the project is about.</td>
    <td><a href="#why-this-project-matters"><strong>Why It Matters</strong></a><br>The technical value behind the project.</td>
  </tr>
  <tr>
    <td><a href="#project-goal"><strong>Project Goal</strong></a><br>What the system was designed to achieve.</td>
    <td><a href="#studied-topics"><strong>Studied Topics</strong></a><br>Main concepts practiced during development.</td>
  </tr>
  <tr>
    <td><a href="#features"><strong>Features</strong></a><br>What was implemented.</td>
    <td><a href="#visual-demo"><strong>Visual Demo</strong></a><br>Screenshots of the application and database.</td>
  </tr>
  <tr>
    <td><a href="#database-modeling"><strong>Database Modeling</strong></a><br>Tables and data organization.</td>
    <td><a href="#php-integration"><strong>PHP Integration</strong></a><br>How the application connects to MySQL.</td>
  </tr>
  <tr>
    <td><a href="#technology-stack"><strong>Technology Stack</strong></a><br>Tools and technologies used.</td>
    <td><a href="#key-learnings"><strong>Key Learnings</strong></a><br>Main lessons from the project.</td>
  </tr>
  <tr>
    <td><a href="#future-improvements"><strong>Future Improvements</strong></a><br>Possible next steps.</td>
    <td><a href="#final-note"><strong>Final Note</strong></a><br>The main takeaway from the project.</td>
  </tr>
</table>

---

<a id="overview"></a>

## Overview

This project is a web application designed to manage business expenses through a relational database.

The application allows expense records to be submitted through a web form and stored in a MySQL database. The main focus of the project was not only the interface, but the structure behind it: database design, table organization, data persistence, and the connection between PHP and MySQL.

The system was developed using XAMPP as the local environment and MySQL Workbench for database modeling and management.

---

<a id="why-this-project-matters"></a>

## Why This Project Matters

Business systems depend heavily on well-structured data.

This project helped me understand how information entered by a user in a form becomes persistent data inside a relational database.

It also brought together important web development concepts:

- Database modeling;
- Table creation and relationships;
- Backend connection with MySQL;
- Data submission through forms;
- CRUD operations;
- Local development with XAMPP;
- Basic deployment workflow.

> [!NOTE]
> The application interface was developed with AI assistance, but the main learning focus was database structure, MySQL modeling, and PHP integration through XAMPP.

---

<a id="project-goal"></a>

## Project Goal

The objective was to develop a web application for a company that needed to register and organize business expenses.

The system had to:

- Allow expense registration;
- Store data in a relational database;
- Use organized database tables;
- Connect the web application to MySQL;
- Persist form data correctly;
- Provide a base structure for financial control.

---

<a id="studied-topics"></a>

## Studied Topics

During the project, I practiced:

- Relational database modeling;
- Creation of tables and relationships in MySQL;
- PHP integration with MySQL using PDO;
- Data manipulation through HTML forms;
- HTTP POST form submission;
- Basic CRUD concepts;
- Web application structure;
- Local development using XAMPP;
- Basic deployment using InfinityFree.

---

<a id="features"></a>

## Features

The project includes:

- Expense registration form;
- Data submission using POST;
- PHP backend processing;
- MySQL database connection using PDO;
- Expense data persistence;
- Database organized by branches, categories and budgets;
- Confirmation message after successful submission;
- Visual validation of stored data in the database.

---

<a id="visual-demo"></a>

## Visual Demo

### Application Interface

Main screen of the expense registration system.

![Application Interface](./assets/aplicacaoWEB.png)

---

### Completed Form

Example of the form filled with business expense data.

![Completed Form](./assets/aplicacaoPreenchida.png)

---

### Successful Submission

Confirmation message after saving the expense data.

![Successful Submission](./assets/resultadoForms.png)

---

### Stored Data in MySQL

Expense record stored in the relational database.

![Stored Data](./assets/resultado.png)

---

### Expenses Table

Structure of the `despesas` table in MySQL.

![Expenses Table](./assets/tabelaDespesas.png)

---

### PHP Database Connection

PHP file responsible for connecting the application to MySQL.

![PHP Connection](./assets/conexaoPHP.png)

---

<a id="database-modeling"></a>

## Database Modeling

The database created for this project was:

```text
financeiro_filiais
```

The model was organized around expense control for company branches.

Main tables:

| Table | Purpose |
|---|---|
| `despesas` | Stores expense records submitted through the form |
| `filiais` | Stores company branch information |
| `categorias_despesa` | Stores expense categories |
| `subcategorias_despesa` | Stores more specific expense classifications |
| `orcamentos_mensais` | Stores monthly budget information |

This structure helps separate responsibilities and makes the database easier to maintain and expand.

---

<a id="php-integration"></a>

## PHP Integration

The application connects to MySQL using PHP with PDO.

PDO was used because it provides a safer and more organized way to connect to a database and execute SQL operations.

The integration flow works like this:

```text
User fills the form
        |
        v
Form sends data using POST
        |
        v
PHP receives the data
        |
        v
PDO connects to MySQL
        |
        v
SQL statement inserts data
        |
        v
Expense is stored in the database
```

This flow helped me understand how frontend forms communicate with backend logic and how data is persisted in a relational database.

---

<a id="technology-stack"></a>

## Technology Stack

| Category | Tools |
|---|---|
| Database | MySQL, MySQL Workbench |
| Backend | PHP, PDO |
| Local Server | XAMPP, Apache, MySQL |
| Editor | VS Code |
| Deployment | InfinityFree |
| Assistance | AI-assisted interface development |

---

## What Was Requested

The requested task was to develop a web application for a company that could:

- Register expenses;
- Store expense data in a relational database;
- Use an organized table structure;
- Integrate the application with the database.

---

## What Was Delivered

The project delivered:

- Creation of the `financeiro_filiais` database;
- Modeling of the main database tables;
- Web form for expense registration;
- PHP integration with MySQL using PDO;
- Data persistence in the database;
- Basic deployment of the application;
- Organized project structure.

---

<a id="key-learnings"></a>

## Key Learnings

This project helped me consolidate important concepts about databases and web applications:

- How to structure a relational database for a real use case;
- How to organize tables according to business needs;
- How PHP connects to MySQL using PDO;
- How form data is sent and processed;
- How data is persisted in a database;
- Why database modeling matters before implementation;
- How local development works with XAMPP;
- Basic notions of web deployment.

---

<a id="future-improvements"></a>

## Future Improvements

Possible improvements for this project include:

- Add full CRUD operations for expenses;
- Add edit and delete features;
- Add user authentication;
- Improve form validation;
- Add filters by branch, category and date;
- Add expense reports and charts;
- Improve interface responsiveness;
- Add environment variables for database credentials;
- Improve deployment structure;
- Add documentation for the database schema.

---

<a id="final-note"></a>

## Final Note

This project was important because it made the connection between application and database more concrete.

The main takeaway was understanding that a web system is not only about what appears on the screen. The real structure is also in how data is modeled, stored, validated and retrieved.

Even with AI assistance during the interface development, the most valuable part of this project was practicing database modeling and understanding how PHP communicates with MySQL.

---

## License

This project was developed for learning purposes.
