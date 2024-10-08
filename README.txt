Project Title

Table of Contents:
- Description
- Installation
- Hyperparameters
- Acknowledgments

Description:
The objective of this project is to implement a Bayesian method based on the TrueSkill ranking system to estimate the skill levels of players involved in competitive scenarios. The proposed method will be evaluated using real-world data and compared against alternative approaches.

Installation:
1. Installing requirements:
   Run the following command to install the necessary dependencies:
   
   pip install -r requirements.txt

2. Open the Jupyter Notebook:
   After installing the dependencies, start Jupyter Notebook by running the following command:
   
   jupyter notebook

3. Navigate to the notebook file:
   In your browser, navigate to the project directory and open the notebook file `runme.ipynb`.

4. Set the hyperparameters:
   In the second cell of the notebook, you will find the hyperparameters. Adjust these values to your desired settings before running the notebook. Default values are provided, but feel free to modify them as needed:
   - dataset_path = "SerieA.csv"
   - mu_1 = 25
   - mu_2 = 25
   - sigma_1 = 25/3
   - (other hyperparameters...)

5. Run the notebook.

6. Review the results.

Hyperparameters:
In this section, you need to set the values for the hyperparameters before running the notebook cells. Below are the key hyperparameters you need to adjust:

- dataset_path: Path to the dataset file used in the analysis.
  - Default: "SerieA.csv" (can be changed to "Extension_data.csv" if needed).
  
- mu_1: Initial mean for first team's skill level.
  - Default: 25

- mu_2: Initial mean for second team's skill level.
  - Default: 25

- sigma_1: Initial standard deviation for first team's skill level.
  - Default: 25/3

- sigma_2: Initial standard deviation for second team's skill level.
  - Default: 25/3

- sigma_t: Standard deviation for the t given s1 and s2
  - Default: 25/6

- iterations: Number of iterations for the Gibbs Sampler
  - Default: 1200

- burn_in: Number of initial samples to discard (burn-in period).
  - Default: 25

- num_seeds: The seed to use for randomizing the order of the matches.
  - Default: 42

- predict_epsilon: Tolerance value to consider a match as a draw.
  - Default: 0.025

- t_epsilon: Tolerance value based on the true skill deviation to consider a match as a draw.
  - Default: sigma_t / 15 (calculated dynamically)

Make sure to review and modify these values in the corresponding cell of the Jupyter Notebook before running the code.

Acknowledgments:
This document serves as the instructional guide for the project assignment for the course Advanced Probabilistic Machine Learning, 1RT705/1RT003.
