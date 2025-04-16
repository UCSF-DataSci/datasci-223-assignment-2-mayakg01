## Data Analysis Explanation
1.**Analysis Approach**
- The script converted the patients_large csv file to parquet format using polars
- Categorized BMI into 4 categories: underweight, normal, overweight, & obese
- Excluded BMI values over 60 or under 10, as these are not logical or common BMI values for patients
- Patients were categorized by BMI range using groupby()
- Found the mean age and glucose values for patients in each BMI range

### Insights
2. **Patterns & Observations**
- Correctly outputted a table containing 4 columns: bmi_range, avg_glucose, patient_count, avg_age
- BMI categorized into 4 categories
- The highest avg glucose by group was in the obese category, with a value of 126.03, while the lowest avg glucose was in the underweight category, with a value of 95.195
- The greatest number of patients were in the obese category, with the fewest in the underweight category
- The normal, overweight, and obese categories had fairly similar average ages, with the youngest average age in the underweight category