# README #

This repository holds all the relevant code for the execution of the questions related to MELI's Challenge. Here you'll find the anwers to questions one to four.

### What is this repository for? ###

**<u>Quick summary</u>**

The script structure is at it follows:
* 0n_name_question_solved.ipynb:     
    * Example: _01_ofertas_relampago.ipynb_ correspond to the solution of the first question of the challenge.

### How do I get set up? ###

**<u>Summary of set up</u>**
* First, you need to install the requirements.
`pip install -r requirements.txt`
* Folders:
  * `Files`: Here all your data sources should be clearly stated. The `.csv` related to the challenge must be save in this folder. To reproduce the solution, you must have the following files provided by MELI:
    * ofertas_relampago.csv
    * ordenamiento.csv
    * items_titles.csv
    * items_titles_test.csv
  * `Notebooks`: Inside this folder you will find the notebooks needed to run each question.

### Environment ###

This project was develop on a MacOS environment (BigSur version 11.6.8) using Python version 3.10.0.
A computer with at least 16 GB of RAM is recommended.

### Instructions ###

Each notebook have a certain structure and outputs. These are the following:

* _01_ofertas_relampago.ipynb_: After the `.csv` file is loaded, cell by cell you will found the corresponding information related to numerical and categorical columns. Subsequently, some questions associated with the data are available, and comments are left.
* _02_ordenar_productos.ipynb_: After the `.csv` file is loaded, and calling the functions, the output and execution time of the algorithm will be found after calling the sort_dataframe function that is in charge of orchestrating the whole process.
* _03_similitud_productos.ipynb_: After loading the `.csv` file, and calling the functions, for simplicity and since the execution times were considerably high, I built a function that is given the dataframe and a particular item_title, with this it returns a dataframe with the comparison of the item_title and the rest of the dataset along with the similarity score.
* _04_forecast.ipynb_: After loading the `.csv` file, and calling the functions, you will find the results obtained after training the model and making the predictions. Two strategies were used here, a model for each category and a multi-category model.