Medical Device Utilization (2025)
This project analyzes synthetic healthcare data to support strategic planning and resource allocation for medical equipment in hospitals and clinics. Using a Power BI dashboard, the analysis explores trends in device usage across facilities, patient demographics, and medical procedures. The dashboard offers insights such as the most used devices, average usage time, forecasted demand, and usage breakdown by gender and healthcare facility. It also highlights the top procedures associated with specific devices and allows drillthrough interactions for focused analysis. The goal is to empower healthcare administrators with validated, actionable information to optimize equipment distribution and improve patient care outcomes.

Background Information
Medical equipment plays a critical role in healthcare delivery, directly impacting diagnosis, treatment, and recovery. However, poor resource allocation often leads to device underutilization or shortages. This project addresses that challenge using data-driven strategies derived from synthetic health records. Synthea™, a synthetic patient generator, was used to simulate real-world hospital and patient scenarios. It provides rich, realistic datasets compliant with privacy standards. Through this project, healthcare decision-makers can visualize equipment demand, predict future needs, and make informed choices on medical device management across various facilities and departments.

Dataset Source
The dataset used in this project was generated using Synthea, a synthetic health data engine.

Tables Used:

devices

procedures

encounters

patients

organizations

(Supporting: careplans, medications, observations)

Tool Used
Microsoft Power BI
Used for data loading, cleaning, transformation, and interactive visualization.

Data Preparation Steps
Import Data:

Imported multiple .csv exports from Synthea output folders.

Loaded into Power BI using the folder connection method.

Pre-Processing in Power BI:

Removed empty or irrelevant columns (e.g., license).

Checked data types and cleaned nulls.

Renamed columns for clarity and standardization.

Created Relationships:

Linked devices, procedures, encounters, and patients using patient and encounter IDs.

Calculated Fields:

DeviceUsageTimeDays = Date difference between START and STOP

Year = Extracted from START for forecasting

Drillthrough Setup:

Enabled device-specific page with focused metrics like usage by gender, forecast, and top procedures.

Dashboard Features
KPI Cards: Devices Used, Total Procedures, Facility Count

Bar Charts: Device Utilization, Procedures by Device, Facilities by Device

Map: Device usage by location

Pie Chart: Usage by Gender

Line Chart: Forecast of Demand

Drillthrough Page: Deep insights into any selected device
