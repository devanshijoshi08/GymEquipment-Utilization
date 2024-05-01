## Optimizing Group Fitness Class Utilization

### Project Overview
This project focuses on predicting attendance in group fitness classes to optimize class schedules and utilization rates at GoalZone, a fitness club chain. By accurately predicting class attendance, GoalZone aims to reduce no-shows, maximize class availability, and improve overall member satisfaction.

### Dataset Description
The dataset includes details about gym class bookings, member characteristics, and class attendance:

- **booking_id**: Unique identifier for the booking.
- **months_as_member**: Number of months the individual has been a member.
- **weight**: Member's weight in kilograms.
- **days_before**: Number of days the booking was made before the class.
- **day_of_week**: Day of the week the class is scheduled.
- **time**: Time of day the class is scheduled (AM or PM).
- **category**: Type of fitness class.
- **attended**: Whether the member attended the class (1) or not (0).

### Prerequisites
You need to have Python installed on your system along with the necessary libraries used in the project. You can install all required libraries using the following command:
```bash
pip install -r requirements.txt
```

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/devanshijoshi08/GymEquipment-Utilization.git
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
Open `EquipmentUtilization.ipynb` in Jupyter Notebook to view the analysis.

## Methodology
The analysis involves the following key steps:
1. **Data Preprocessing**: Handling missing values, encoding categorical variables, and normalizing data.
2. **Feature Engineering**: Creating new features that might help improve model accuracy.
3. **Model Selection**: Using Grid Search CV to find the best hyperparameters for RandomForestClassifier, LogisticRegression, and GradientBoostingClassifier.
4. **Evaluation**: Assessing model performance through accuracy, precision, recall, and a confusion matrix.

## Results
The best-performing model was GradientBoostingClassifier with an accuracy of 74.22%. The results indicate that:
- True Negatives (correct prediction of non-attendance): 277
- True Positives (correct prediction of attendance): 57
- The model was particularly effective in predicting non-attendance.

## Conclusion
The analysis provides insights into class attendance patterns, helping to better schedule and manage fitness classes. Future work will focus on integrating these models into a real-time booking system and further refining predictions with additional data.

