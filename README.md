IoT Sensor Data Analysis using NumPy

📌 Project Overview

This project demonstrates how to analyze IoT sensor data using Python and the NumPy library.

The program processes a collection of sensor readings and performs basic statistical operations such as calculating the mean, median, minimum, maximum, and standard deviation.

It also identifies sensor readings that exceed a predefined threshold.

🎯 Objectives

- Analyze IoT sensor readings using Python.
- Perform statistical calculations using NumPy.
- Identify minimum and maximum sensor values.
- Calculate the mean, median, and standard deviation.
- Detect sensor readings exceeding a specified threshold.

🛠️ Technologies Used

- Programming Language: Python
- Library: NumPy
- Concepts: Arrays, Statistical Analysis, Boolean Indexing, Threshold Detection

✨ Features

1. Sensor Data Storage: Stores sensor readings in a NumPy array.
2. Mean Calculation: Calculates the average sensor reading.
3. Median Calculation: Identifies the middle value of the dataset.
4. Minimum and Maximum: Finds the lowest and highest sensor readings.
5. Standard Deviation: Measures the variation in sensor readings.
6. Threshold Detection: Identifies readings exceeding the specified threshold.

💻 Source Code

import numpy as np

sensor_data = np.array([
    24.5, 25.1, 26.3, 27.0, 28.2,
    29.1, 27.8, 26.5, 25.7, 30.2
])

print("Sensor Data:", sensor_data)

print("Mean :", round(np.mean(sensor_data), 2))
print("Median :", round(np.median(sensor_data), 2))
print("Minimum :", np.min(sensor_data))
print("Maximum :", np.max(sensor_data))
print("Std. Dev. :", round(np.std(sensor_data), 2))

threshold = 28.0

high_values = sensor_data[sensor_data > threshold]

print("Values above", threshold, ":", high_values)

📊 Sample Output

Sensor Data: [24.5 25.1 26.3 27.  28.2 29.1 27.8 26.5 25.7 30.2]
Mean : 27.04
Median : 26.75
Minimum : 24.5
Maximum : 30.2
Std. Dev. : 1.74
Values above 28.0 : [28.2 29.1 30.2]

⚙️ Installation and Execution

Step 1: Install Python

Ensure Python is installed on your computer.

Step 2: Install NumPy

Open your terminal and execute:

pip install numpy

Step 3: Run the Program

Save the Python code as:

sensor_analysis.py

Execute the program using:

python sensor_analysis.py

🔍 Working Principle

Step 1: Data Collection

Sensor readings are stored in a NumPy array.

Step 2: Statistical Analysis

NumPy functions calculate the mean, median, minimum, maximum, and standard deviation.

Step 3: Threshold Comparison

Each sensor reading is compared against a threshold of 28.0.

Step 4: Result Generation

The program displays the statistical results and readings exceeding the threshold.

🌍 Applications

- IoT Sensor Monitoring
- Environmental Data Analysis
- Temperature Monitoring Systems
- Smart Home Monitoring
- Industrial Sensor Data Analysis

🚀 Future Enhancements

- Integrate real-time IoT sensor readings.
- Visualize sensor data using Matplotlib.
- Implement automatic alerts for abnormal readings.
- Store sensor readings in a database.
- Develop a web-based monitoring dashboard.

📚 Learning Outcomes

Through this project, I gained practical experience in:

- Working with NumPy arrays.
- Performing statistical calculations.
- Filtering data using Boolean indexing.
- Implementing threshold-based data analysis.
- Understanding basic IoT data processing concepts.

👨‍💻 Author

KARTHICK B

Computer Science and Engineering
Chennai Institute of Technology

📄 Conclusion

This project demonstrates a simple and effective approach to analyzing sensor data using Python and NumPy. It provides a foundation for developing more advanced IoT monitoring and data analysis applications.