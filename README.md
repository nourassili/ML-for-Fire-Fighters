Overview
This project focuses on improving emergency response performance for the City of Rochester Fire Department (RFD) through advanced data analysis and predictive modeling. By leveraging geospatial data, historical incident records, and state-of-the-art machine learning techniques, this initiative aims to enhance resource allocation, optimize deployment strategies, and reduce response times, ensuring operational excellence and community safety.

Key Features
Geospatial Analysis: Evaluate fire station coverage and incident hotspots using interactive maps.
Predictive Modeling: Forecast monthly incident counts to prepare for future demands.
Resource Optimization: Propose unit relocations and workload redistributions based on historical data.
Low-Acuity Response Program: Suggest a pilot program to handle non-emergency calls and alleviate strain on critical resources.
Datasets
Incident Data: Details about emergencies, including type, location, and response actions.
Station Apparatus Data: Information on station-specific resources and units.
Geospatial Data: Shapefiles for fire station locations to enable spatial analysis.
Methodology
Data Preprocessing: Cleaned and imputed missing values in incident and geospatial datasets.
Exploratory Data Analysis: Identified seasonal trends, peak hours, and incident types across RFD.
Predictive Modeling:
Forecasted incident counts using the Prophet model.
Incorporated feature engineering and lagged variables for improved accuracy.
Interactive Maps: Developed visualizations to analyze response times and incident distributions.
Key Insights and Recommendations
Seasonal Trends: Summer months and late afternoon hours see the highest incident rates.
Resource Allocation: Relocated units to align with high-incident zones.
Proposed Initiatives: Introduced a low-acuity response program to address non-emergency calls.
Performance Metrics
The project achieved high forecasting accuracy with key metrics, including:

RMSE: 5.835
MAPE: 18.945%
R²: ~85% across all stations
How to Use
Setup
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/rochester-fire-response.git
cd rochester-fire-response
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Running the Model
Train the model:
bash
Copy
Edit
python train_model.py
Visualize results:
bash
Copy
Edit
python generate_visuals.py
Interactive Maps
Access the interactive maps to explore station coverage and response dynamics:
bash
Copy
Edit
python run_interactive_maps.py
Future Work
Enhanced Predictive Models: Incorporate external data like traffic and weather for improved response time predictions.
Low-Acuity Program Implementation: Conduct feasibility studies and pilot testing.
Real-Time Dashboards: Build user-friendly dashboards for better decision-making.
Contact
For inquiries, contact the project team at nassili@u.rochester.edu
