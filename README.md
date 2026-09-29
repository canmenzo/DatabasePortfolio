# 🗄️ Database Portfolio

[![license](https://img.shields.io/github/license/canmenzo/DatabasePortfolio)](LICENSE) ![coursework](https://img.shields.io/badge/coursework-archived-lightgrey) ![bash](https://img.shields.io/badge/bash-scripts-4EAA25?logo=gnubash&logoColor=white) ![database](https://img.shields.io/badge/database-MySQL-4479A1?logo=mysql&logoColor=white)

Archived coursework from spring 2021 (Activity 7): Bash scripts that query a MySQL `sales` database of car sales and turn the results into per-model reports. Kept as a learning project.

### ✨ What's in it
- ⚙️ `q01/q01.sh`: writes the `env_mysql` file with the MySQL user, password (a `your_password_here` placeholder; set your own) and report/archive paths, and symlinks it into the other question folders
- 🔎 `q02/q02.sh <year> <model> <all|new|used>`: count of cars sold plus total dealer cost, sale price and list price for one model and year
- 📋 `q03/q03.sh <model>`: checks the model name against the database, then builds a 2010 to 2016 sales report for all, new and used cars
- 💰 `q04/q04.sh <model>`: the same report with profit, discount, and average profit and discount per car added
- 📦 `q05/q05.sh`: runs `q04.sh` for every model, saves the reports to `~/reports` and tars them into `~/archive/models.tar`
- 🗂️ `q01/*.txt`: sample reports for each Honda model; `lab07.txt`: the grader output; `.s01.sh` to `.s05.sh`: earlier versions of the scripts

### 🚀 Running it
The `sales` database is not in this repo, so the scripts will not run as-is. They expect a MySQL server with `sales_2010` to `sales_2016` tables (`model_name`, `sales_type`, `dealer_cost`, `price_sold`, `price_list`) and some scripts use hard-coded `~/class/a07/...` paths from the class server.

### 📄 License
MIT
