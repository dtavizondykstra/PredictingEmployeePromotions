# PredictingEmployeePromotions
This project aims to develop a data-driven approach to predict employee promotions within an organization. By leveraging machine learning techniques, we can enhance fairness, reduce biases, and optimize the allocation of training resources.

## Table of Contents
* Introduction
* Project Structure
* Dataset
* Installation
* Usage
* Results
* Contributing
* License

## Introduction
Traditional methods of employee promotion often rely on subjective evaluations and recommendations, which can introduce biases and inefficiencies. This project utilizes data analytics and machine learning to predict whether an employee should be promoted, based on various factors such as performance metrics, demographics, and training scores.

## Project Structure
```
├── data
│   ├── train.csv
│   └── test.csv
├── main.ipynb
├── README.md
```

* `data/`: Directory containing the training and testing datasets.
* `main.ipynb`: Jupyter notebook with the code for data analysis and model development.
* `README.md`: Project documentation.

## Dataset
The datasets used in this project are:
* Training Dataset (train.csv): Contains employee data with 14 columns, including the target variable is_promoted.
* Testing Dataset (test.csv): Contains similar employee data without the target variable.

## Key Variables:
* employee_id: Unique ID for each employee
* department: Department of the employee
* education: Education level of the employee
* gender: Gender of the employee
* no_of_trainings: Number of trainings completed
* age: Age of the employee
* previous_year_rating: Employee's rating for the previous year
* length_of_service: Length of service in years
* KPIs_met >80%: If KPIs met above 80%
* awards_won?: If awards won during the previous year
* avg_training_score: Average score in current training evaluations
*  is_promoted: Promotion status (Target variable)

## Installation
Prerequisites
```
Python 3.x
Jupyter Notebook or Google Colab
Required Python libraries (listed below)
```

Required Libraries
```
bash
Copy code
numpy
pandas
matplotlib
seaborn
scikit-learn
imbalanced-learn
```

## Installing Libraries
You can install the required libraries using pip:
```
pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn
```

## Usage
Clone the Repository
```
git clone https://github.com/yourusername/employee-promotion-prediction.git
```

## Navigate to the Project Directory
```
cd employee-promotion-prediction
```

## Place the Datasets
* Ensure that train.csv and test.csv are placed inside the data/ directory.
Open the Jupyter Notebook
* Launch Jupyter Notebook and open main.ipynb.
  * Alternatively, you can upload main.ipynb to Google Colab.

## Run the Notebook
* Execute the cells sequentially to perform data analysis, preprocessing, model training, and evaluation.
Results

## Data Preprocessing:
* Handled missing values by imputing with the mode.
  * Performed outlier detection and removed insignificant outliers.
  * Conducted univariate, bivariate, and multivariate analyses to understand data distributions and relationships.
  * Created new features (sum_metric, total_score) through feature engineering.
  * Encoded categorical variables and scaled numerical features.

## Modeling:
* Addressed class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).
* Split the data into training and validation sets.
* Trained a Decision Tree Classifier.
* Achieved training accuracy of approximately 100% and testing accuracy of approximately 98%.

## Evaluation:
* Evaluated the model using confusion matrix and classification report.
* Observed high precision and recall rates, indicating effective prediction capability.

## Contributing
* Contributions are welcome! Please follow these steps:
  * Fork the repository.
  * Create a new branch:
    
```
git checkout -b feature/your-feature-name
```

  * Commit your changes:
```
git commit -m 'Add your commit message'
```

  * Push to the branch:
```
git push origin feature/your-feature-name
```
  * Open a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
