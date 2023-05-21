
# Patient Information Processing

This Python script reads, processes, and aggregates patient appointment data for a healthcare application. The data includes patient demographic information, consultation details, and appointment specifics.


## Data Processing

Here are the primary data transformations and processing applied to the dataset:

- Reading the JSON file and transforming it into a pandas DataFrame for easy processing.

- Renaming and selecting required columns.

- Creating a full name field by concatenating first and last name fields.

- Converting gender field to a more descriptive format, mapping 'M' and 'F' to 'male' and 'female' respectively. Any other values are classified as 'others'.

- Validating phone numbers using the phonenumbers library and recording the validity as a boolean field.

- Hashing phone numbers using SHA-256 for privacy and data protection.

- Converting date of birth field to datetime and calculating age.

- Calculating the number of medicines, active medicines, and inactive medicines for each patient.

- Extracting the names of active medicines.

- The transformed data is then saved into a CSV file with the delimiter '~'.
## Data Aggregation

The script also performs the following aggregations:

- Calculating the average age of patients.

- Counting patients by gender.

- Counting the number of valid phone numbers.

- Counting unique appointments.

- Summing up the total number of medicines, active and inactive.

- The aggregated data is saved into a JSON file.
## Data Visualisation

Lastly, a pie chart of patient gender distribution is generated using Matplotlib.

![Chart](https://github.com/Gaurang105/Bajaj_Finserv_Assignment/blob/master/screenshot/chart.png?raw=true)
