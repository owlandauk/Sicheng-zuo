## Data

The provided data is structured as follows:
![Data Structure Diagram](Data/schema.png)


The function you write should return data as described below.

There should be a unique row for each daily entry combining health metrics and supplement usage.

Where missing values are permitted, they should be in the default Python format unless stated otherwise.

| Column Name        | Description |
|--------------------|-------------|
| user_id            | Unique identifier for each user. </br>There should not be any missing values. |
| date               | The date the health data was recorded or the supplement was taken, in date format. </br>There should not be any missing values. |
| email              | Contact email of the user. </br>There should not be any missing values. |
| user_age_group  | The age group of the user, one of: 'Under 18', '18-25', '26-35', '36-45', '46-55', '56-65', 'Over 65' or 'Unknown' where the age is missing.|
| experiment_name    | Name of the experiment associated with the supplement usage. </br>Missing values for users that have user health data only is permitted. |
| supplement_name    | The name of the supplement taken on that day. Multiple entries are permitted. </br>Days without supplement intake should be encoded as 'No intake'. |
| dosage_grams       | The dosage of the supplement taken in grams. Where the dosage is recorded in mg it should be converted by division by 1000.</br>Missing values for days without supplement intake are permitted. |
| is_placebo         | Indicator if the supplement was a placebo (true/false). </br>Missing values for days without supplement intake are permitted. |
| average_heart_rate | Average heart rate as recorded by the wearable device. </br>Missing values are permitted. |
| average_glucose    | Average glucose levels as recorded on the wearable device. </br>Missing values are permitted. |
| sleep_hours        | Total sleep in hours for the night preceding the current day’s log. </br>Missing values are permitted. |
| activity_level     | Activity level score between 0-100. </br>Missing values are permitted. |
