# Credit Score Prediction

This project focuses on predicting a person's credit score based on their financial data using machine learning models like Random Forest Classifier. 
The dataset used contains several features such as Annual Income, Monthly Salary, Credit Utilization Ratio, and more.
The project explores data visualization with Plotly and performs predictive analysis.

Credit score prediction is important in financial services as it helps banks, loan institutions, and other financial entities assess a person's creditworthiness. This project utilizes a dataset that includes features such as annual income, number of credit cards, outstanding debt, and more to predict a person's credit score. The main objective is to build a machine learning model that accurately classifies credit scores into three categories: `Poor`, `Standard`, and `Good`.

## Project Structure

```bash
├── data/                    # Directory for datasets
│   └── train1.csv            # Training dataset used for model building
├── images/                   # Directory for images (optional for visualizations)
├── models/                   # Saved trained models (optional)
├── src/                      # Directory for source code
│   └── credit_score_model.py  # Python file for the model and analysis
├── README.md                 # Project documentation
└── requirements.txt          # List of dependencies
```

## Requirements

This project uses several Python libraries. The required packages can be installed via the `requirements.txt` file. Major libraries include:

- `pandas`
- `numpy`
- `plotly`
- `matplotlib`
- `scikit-learn`

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/credit-score-prediction.git
   ```

2. Navigate to the project directory:

   ```bash
   cd credit-score-prediction
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Dataset

The dataset used is provided in the `data/train1.csv` file. It contains several features related to a person's financial history, which are used to predict their credit score.

### Features:
- **Annual_Income**: The yearly income of the individual.
- **Monthly_Inhand_Salary**: Salary received after deductions.
- **Num_Bank_Accounts**: The number of active bank accounts.
- **Num_Credit_Card**: Number of credit cards held by the individual.
- **Interest_Rate**: Average interest rate on loans.
- **Num_of_Loan**: Total number of loans taken by the individual.
- **Delay_from_due_date**: Average delay in payment for credit cards.
- **Num_of_Delayed_Payment**: Total number of delayed payments.
- **Outstanding_Debt**: Amount of debt unpaid.
- **Credit_History_Age**: Age of the credit history.
- **Monthly_Balance**: Monthly remaining balance after expenses.
- **Credit_Score**: Target variable — Poor, Standard, Good.

## Model Training

The project uses a `RandomForestClassifier` model for classification tasks. The training process uses a portion of the dataset split into training and testing sets, and the model's accuracy is evaluated.

## Usage

To run the project, follow these steps:

1. Ensure all required packages are installed (see the [Requirements](#requirements) section).
2. Run the Python file for exploratory data analysis and model training:

   
   python src/credit_score_model.py
   
3. The script will prompt for user input to predict a credit score based on features like Annual Income, Monthly Inhand Salary, and others. Input the values as requested, and the model will output a predicted credit score.

Example:

Annual Income: 50000
Monthly Inhand Salary: 4000
Number of Bank Accounts: 3
Number of Credit cards: 2
Interest rate: 8.5
Number of Loans: 1
Average number of days delayed by the person: 2
Number of delayed payments: 1
Credit Mix (Bad: 0, Standard: 1, Good: 3) : 1
Outstanding Debt: 15000
Credit History Age: 5
Monthly Balance: 1000

Predicted Credit Score = ['Standard']
```

