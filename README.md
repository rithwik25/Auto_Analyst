# Multi-Agent Supervisor System for Data Analysis

This project implements a multi-agent system with a supervisor that coordinates between specialized agents to handle different types of data-related queries.

## Features

- **SQL Agent**: Handles database queries and schema exploration
- **Data Visualizer**: Creates charts and visualizations
- **Forecaster**: Performs time-series forecasting
- **Summarizer**: Provides concise summaries of data
- **Intelligent Supervisor**: Routes queries to the appropriate agents

## Prerequisites

- Python 3.10
- OpenAI API key
- SQLite database (automatically created from CSV)

## Installation

1. Clone this repository
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate    # Windows
3. Install Dependencies
    ```bash
    pip install -r requirements.txt
4. Create a .env file with your API keys
    ```bash
    OPENAI_API_KEY=your_openai_key
    TAVILY_API_KEY=your_tavily_key

## Usage

1. Place your salary_data.csv in the project root
2. Run the ipynb cells

## Project Structure

project/  
├── supervisor.ipynb       # Main ipynb file "\n"  
├── salary_data.csv        # Input data file  
├── salaries.db            # Generated SQLite database  
├── requirements.txt       # Python dependencies  
├── README.md              # This file  
└── .env                   # Environment variables  

## Limitations

* Requires properly formatted CSV input
* Forecasting functionality needs time-series data
* Visualization output paths are hardcoded
