# Data Dictionary
## Dataset Field Definitions
1. **Data Value (data_value)**
   - Type: Numeric
   - Description: The recorded value of a specific environmental or health indicator for a given geographic unit and time period.

2. **Geo Join ID (geo_join_id)**
   - Type: Text
   - Description: Geographic identifier used to link the dataset with spatial boundary files for mapping purposes.

3. **Name (name)**
   - Type: Text
   - Description: The name of the indicator being measured. Represents the variable category for each observation.

4. **Geo Type Name (geo_type_name)**
   - Type: Categorical (Ordered Factor)
   - Description: Specifies the geographic aggregation level at which the data is reported.

5. **Unique ID (unique_id)**
   - Type: Text
   - Description: A unique identifier assigned to each record in the dataset.

6. **Indicator ID (indicator_id)**
   - Type: Numeric
   - Description: A numerical code representing each distinct indicator across time and geography.

7. **Geo Place Name (geo_place_name)**
   - Type: Text
   - Description: The name of the geographic area associated with the observation.

8. **Message (message)**
   - Type: Text
   - Description: Supplementary notes associated with the data value.

9. **Measure Info (measure_info)**
   - Type: Text
   - Description: Provides information about the unit or measurement definition associated with the indicator.

10. **Start Date (start_date)**
    - Type: Date
    - Description: The starting date of the observation period.

11. **Time Period (time_period)**
    - Type: Text
    - Description: Describes the temporal coverage of the observation.
