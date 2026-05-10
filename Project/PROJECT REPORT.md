# **PROJECT REPORT:**

# **SMART PLANTING ASSISTANT**



### **INTRODUCTION:**

The Smart Planting Assistant is a beginner-friendly Python-based application designed to help users choose suitable plants based on their environment and preferences. The system provides recommendations by considering factors such as season, region, available space, and plant type.



The goal of this project is to simplify plant selection for beginners who may not have prior knowledge about gardening or plant requirements.



### **OBJECTIVE:**

* To assist users in selecting plants suitable for their environment
* To provide structured plant information (growth time, soil, water, etc.)
* To offer beginner-friendly gardening tips and essential tools
* To create a simple and interactive command-line application



### **TECHNOLOGIES USED:**

Python (Core programming language)

Pandas (for data handling, filtering and basic calculations like averages)



### **DATASET DESCRIPTION:**

The dataset is manually created and contains information about 20 different plants. Each plant includes:



###### **Plant Name:**

* Season (best growing season)
* Region (suitable area in Pakistan)
* Sunlight Requirement
* Water Requirement
* Growth Duration (in days)
* Soil Type
* Space Requirement
* Plant Type



### **SYSTEM WORKING:**



###### **1. USER INPUT:**

&#x20;  The system takes input for:

* &#x20;Season
* &#x20;Region
* &#x20;Space
* &#x20;Plant Type
* &#x20;Weather condition



###### **2. DATA FILTERING:**

&#x20;  Plants are filtered based on matching conditions:

* Season or “all”
* Region or “all”
* Space type
* Plant type



###### **3. RECOMMENDATIONS:**

&#x20;  Top 5 matching plants are shown with details:

* &#x20;Season
* &#x20;Region
* &#x20;Sunlight
* &#x20;Water
* &#x20;Soil
* &#x20;Space
* &#x20;Growth Time

If no match is found, a friendly message is displayed.



###### **4. IMPORTANT INFORMATION:**

&#x20;Average growth time of selected plants

&#x20;Fastest growing plant



###### **5. GARDENING TOOLS:**

* Trowel
* Shovel
* Hoe
* Shears
* Watering can



###### **6. SMART TIPS:**

&#x20;Indoor/Balcony → use drainage pots

&#x20;Hot weather → water early

&#x20;Cold weather → protect from frost

&#x20;Humid → ensure airflow

&#x20;Dry → maintain moisture



###### **7. DISCLAIMER:**

&#x20;  “Just a heads-up: I'm still learning, double-check anything you're unsure about.”



### **FEATURES:**

* &#x20;Interactive command-line interface
* &#x20;Beginner-friendly design
* &#x20;Simple rule-based logic
* &#x20;Realistic plant dataset
* &#x20;Personalized recommendations
* &#x20;Helpful gardening tips and insights



### **LIMITATIONS:**

* &#x20;Static dataset (not real-time)
* &#x20;Strict filtering may return no results sometimes
* &#x20;No weather API integration
* &#x20;Not machine learning based



### **FUTURE IMPROVEMENTS:**

* &#x20;GUI or web application version
* &#x20;Machine learning-based recommendations
* &#x20;Real-time weather integration
* &#x20;Larger plant dataset
* &#x20;Plant images and care guides



### **CONCLUSION:**

The Smart Planting Assistant helps users choose suitable plants using simple logic and filtering. It is especially useful for beginners and provides a strong foundation for future intelligent gardening systems.

