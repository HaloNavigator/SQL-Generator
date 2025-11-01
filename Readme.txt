This is a fantastic tool! Based on the source code, I've created a comprehensive and professional **README.md** file for your GitHub repository.

The application is a standalone, powerful tool for generating and visualizing SQL queries for a database schema, which appears to be related to the "Halo" IT Service Management platform.

***

# Halo Navigator: SQL Generator & Join Visualiser

A powerful, standalone HTML application designed to simplify the process of writing complex SQL `SELECT` queries for the **Halo** database schema. This tool features an interactive interface for selecting tables/columns, building filters, applying aggregates, and visually mapping database relationships in real-time.

## ✨ Features

* **Interactive Schema Browser**: Easily search and select fields from over 70 known Halo database tables (e.g., `Faults`, `Users`, `Device`, `OrderHead`).
* **Automatic SQL Generation**: Dynamically constructs complete `SELECT`, `FROM`, `INNER JOIN`, `WHERE`, and `GROUP BY` clauses as you make selections.
* **Live Join Visualiser**: A dedicated panel uses **Mermaid.js** to render a live, dynamic flowchart of the tables and join conditions currently included in your query.
    * Includes a button to **Export** the generated visualization as a **PNG** image.
* **Advanced Query Building**:
    * Tools to easily add custom `WHERE` conditions, `GROUP BY` clauses, and aggregate functions (`COUNT`, `SUM`, `AVG`, `MAX`, `MIN`).
    * Specialized filter for ITSM Request Types (Incident, Change, Problem, Service Request) that automatically applies conditions to the `[Faults]` table.
    * Option to view and select from **Possible Joins** or define **Custom Join Conditions**.
* **Export Functionality**: One-click buttons to **Copy** the generated SQL or **Export** it as a `.sql` file.
* **User Experience**: Features a responsive design with a toggle for **Dark/Light Mode**.

---

## 🛠️ Technologies Used

This application is built entirely with frontend technologies, making it a highly portable, zero-dependency tool.

* **HTML5**
* **CSS3** (Custom Styles for a clean, modern UI)
* **Pure JavaScript** (All logic is self-contained)
* **Mermaid.js** (For diagram and chart rendering in the Visualiser)

---

## 🚀 Setup & Installation

Since this application is a single HTML file with all dependencies (CSS, JavaScript, and data) embedded, there is **no installation** required.

1.  **Download** the `Halo_Navigator_SQL_Generator_V6.html` file.
2.  **Open** the file in any modern web browser (Chrome, Firefox, Edge, etc.).

That's it! The application is immediately ready to use.

---

## 💡 Usage

The application is structured into three main columns for an intuitive workflow:

1.  **Schema Panel (Left)**: Search and select the tables and columns you want in your final `SELECT` statement. Selecting a column adds the corresponding table to the join map.
2.  **Filter/Aggregate Panel (Center)**: Use the tools here to add `WHERE` conditions, apply aggregate functions, and define `GROUP BY` clauses.
3.  **Output Panel (Right)**:
    * View the **Generated SQL** in real-time.
    * The **Possible Joins** section automatically suggests relationships between your selected tables. Select the ones you need to include them in the query and the visualiser.
    * The **Visualiser** shows a diagram of how all your selected tables are joined together.
