# Relational Algebra Visualizer

This application is a `Dash`-based tool for visualizing relational algebra queries. It includes an interactive graphical interface for constructing and displaying relational operations using `dash-cytoscape`.

<img width="1000" alt="Screenshot 2025-03-07 at 11 29 52 AM" src="https://github.com/user-attachments/assets/a8b42062-95c0-41d3-8fa2-6d2a7a7c0901" />


## Installation
- Ensure you have:
   - **Python 3.11+**
   - **SQLite3**

- Clone the Repository:
  
   ```bash
   git clone https://github.com/linnerlek/RA-Viz.git
   cd RA-Viz/
   ```
   
- Install Dependencies:
  
   ```bash
   pip3 install -r requirements.txt
   ```
   
- Start the application with:
   ```bash
   python3 app.py
   ```
- Then open your browser and navigate to:
   ```
   http://127.0.0.1:5020
   ```

---

## Adding Custom Databases
The application supports custom SQLite databases. To add your own:
1. **Place your `.db` file** inside the `/databases` folder.
2. Restart the application.
3. Select your new database from the dropdown in the UI.

If the new database doesn't appear, ensure the `.db` file has valid tables.

---
## Supported Operations
This tool supports the following **relational algebra** operations:

| **Operation** | **Description** |
|--------------|----------------|
| `project`   | Selects specific columns |
| `select`    | Filters rows based on conditions |
| `join`      | Combines tables using matching columns |
| `rename`    | Renames columns |
| `union`     | Combines results (removes duplicates) |
| `intersect` | Returns common rows between queries |
| `times`     | Computes the Cartesian product |
| `minus`     | Returns rows from the first query not in the second |
| `aggregate` | Performs `SUM`, `AVG`, `COUNT`, `MIN`, `MAX` |

