<p align="center">
  <a href="" rel="noopener">
 <img src="https://img.pokemondb.net/design/avif/header-lg.avif" alt="Project logo"></a>
</p>
<h3 align="center">Pokémon Pokédex Scraper</h3>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/dnachavez/Pokemon-Pokedex-Scraper.svg)](https://github.com/dnachavez/Pokemon-Pokedex-Scraper/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/dnachavez/Pokemon-Pokedex-Scraper.svg)](https://github.com/dnachavez/Pokemon-Pokedex-Scraper/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)

</div>

---

<p align="center"> This project scrapes the complete Pokémon Pokédex list from a website and saves the data into CSV and SQLite database files. Developed for the Data Engineering Pilipinas challenge.
    <br> 
</p>

## 📝 Table of Contents

- [Problem Statement](#problem_statement)
- [Idea / Solution](#idea)
- [Dependencies / Limitations](#limitations)
- [Future Scope](#future_scope)
- [Setting up a local environment](#getting_started)
- [Usage](#usage)
- [Technology Stack](#tech_stack)
- [Contributing](../CONTRIBUTING.md)
- [Authors](#authors)
- [Acknowledgments](#acknowledgments)

## 🧐 Problem Statement <a name = "problem_statement"></a>

t is useful to design and follow a specific format when writing a problem statement. While there are several options for doing this, the following is a simple and straightforward template often used in Business Analysis to maintain focus on defining the problem.

- IDEAL: To have an automated, reliable, and efficient method to extract and store Pokémon Pokédex data for analysis and usage in various applications.
- REALITY: Currently, there is no easy way to get this data programmatically from the website in a structured format like CSV or a database.
- CONSEQUENCES: Without an automated solution, collecting and using the data becomes time-consuming and error-prone, limiting its potential applications in data analysis, machine learning, and other areas.

## 💡 Idea / Solution <a name = "idea"></a>

This project provides a Python script that scrapes the complete [Pokémon Pokédex](https://pokemondb.net/pokedex/all) list from the Pokémon Database website, cleans the data, and stores it in both CSV and SQLite database formats.

## ⛓️ Dependencies / Limitations <a name = "limitations"></a>

- Dependencies:
  - Python 3.7+
  - requests library for making HTTP requests.
  - beautifulsoup4 for parsing HTML content.
  - pandas for data manipulation and storage.
  - tqdm for displaying a progress bar.
  - sqlite3 for database operations (part of Python Standard Library).

- Limitations:
  - The script relies on the structure of the HTML page. Any changes to the HTML structure of the source website may break the script.
  - Internet connection is required to fetch the data from the website.

## 🚀 Future Scope <a name = "future_scope"></a>

- Automate the script to run at regular intervals and update the database with new Pokémon data.
- Extend the script to include additional data points such as abilities, evolutions, and moves.
- Develop a web interface to display and query the Pokémon data stored in the database.

## 🏁 Getting Started <a name = "getting_started"></a>

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need to have Python 3.7+ installed on your machine. You can download it from [python.org](https://www.python.org/).

### Installing

1. **Clone the repository:**
```
git clone https://github.com/yourusername/pokemon-pokedex-scraper.git
cd pokemon-pokedex-scraper
```

2. **Create a virtual environment and install dependencies:**
```
python -m venv venv
venv\Scripts\activate (Windows)
source venv/bin/activate (Mac/Linux)
pip install requests beautifulsoup4 pandas tqdm
```

3. **Run the script:**
```
python app.ipynb
```

## 🎈 Usage <a name="usage"></a>

After running the script, you will find two files in the project directory:

- pokedex.csv: Contains the complete Pokémon Pokédex data in CSV format.
- pokedex.db: Contains the same data stored in a SQLite database.

## ⛏️ Built With <a name = "tech_stack"></a>

- [Python](https://www.python.org/) - Programming Language
- [Requests](https://pypi.org/project/requests/) - HTTP Library
- [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/) - HTML Parsing Library
- Pandas - Data Manipulation Library
- [tqdm](https://pypi.org/project/tqdm/) - Progress Bar

## ✍️ Authors <a name = "authors"></a>

- [@dnachavez](https://github.com/dnachavez) - Development & Initial work

See also the list of [contributors](https://github.com/dnachavez/Pokemon-Pokedex-Scraper/contributors)
who participated in this project.

## 🎉 Acknowledgments <a name = "acknowledgments"></a>

- Hat tip to [Data Engineering Pilipinas](https://www.facebook.com/groups/dataengineeringpilipinas) Facebook Group
- Inspiration from the [Pokémon Database](https://pokemondb.net/pokedex/all)
