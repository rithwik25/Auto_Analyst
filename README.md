# AI-Driven Data Analysis

### Overview
This project demonstrates the use of LangChain and Python tools to build a sophisticated workflow management system that involves multiple agents (workers) and a supervisor. The system can dynamically assign tasks to workers, route messages, and allow Python-based execution (like SQL queries or data visualizations).

The workflow is designed to handle tasks like:
* Generating SQL queries for database operations.
* Visualizing data using Python scripts.
* Assigning tasks and supervising agents to complete user requests.

### Features
* SQL Developer Agent: An agent that can list tables, query metadata, check SQL query correctness, and execute SQL queries on a database.
* Chart Generator Agent: An agent that executes Python code to generate charts based on data.
* Supervisor Agent: A high-level agent that supervises the workflow, decides which agent should act next, and ultimately finalizes the workflow once all tasks are completed.
* Python REPL Tool: Executes arbitrary Python code for data visualizations and other Python-based tasks.

### Installation
1. Clone the repository:

    git clone https://github.com/rithwik25/Auto_Analyst.git

    cd Auto_Analyst

2. Install the required dependencies:

    pip install -r requirements.txt

3. Install additional libraries if required, such as matplotlib for plotting:

    pip install matplotlib

### Dependencies
* Python 3.10
* langchain library
* langchain_experimental library
* matplotlib for plotting (if visualizations are needed)
* Other required libraries listed in requirements.txt

### Available Tools
1. **python_repl**

    This tool executes Python code locally to generate visualizations (e.g., bar charts, pie charts, etc.). It executes any valid Python code and returns the result as output.

2. **list_tables**
   
    Lists the available tables in the connected database.

3. **tables_schema**
   
    Fetches the schema and sample rows for the provided tables. Useful for understanding the structure of the database.

4. **execute_sql**
   
    Executes an SQL query against the database and returns the results.

5. **check_sql**
   
    Checks the syntax of the SQL query before execution to ensure its validity.

### Example Output

After running a request, such as generating a bar chart, the system will execute the code and save the chart as an image (image.png). It will return the path of the image or any other result based on the task.


   
