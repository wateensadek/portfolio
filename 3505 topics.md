```
# Topic 1: Working with pandas DataFrames
import pandas as pd

data = {
    'Name': ['Wateen', 'Sarah', 'Amira', 'Jonny'],
    'Age': [24, 27, 22, 32],
    'City': ['Halifax', 'Toronto', 'Vancouver', 'Montreal']
}

df = pd.DataFrame(data)
print("DataFrame:")
print(df)

# Add a new column
print("\nAdding a new column:\")
df['Age in 5 Years'] = df['Age'] + 5
print(df)

# Filter rows
print("\nRows where Age > 25:")
filtered_df = df[df['Age'] > 25]
print(filtered_df)

# Topic 2: Visualization
import matplotlib.pyplot as plt

ages = df['Age']
names = df['Name']

plt.bar(names, ages, color='skyblue')
plt.title('Age of Individuals')
plt.xlabel('Name')
plt.ylabel('Age')
plt.show()

# Topic 3: Exploratory Data Analysis (EDA)
print("\nSummary statistics for Age column:")
print(df['Age'].describe())

print("\nChecking for missing values:")
print(df.isnull().sum())

# Topic 4: Single-unit data analysis
single_unit_data = [0.1, 0.5, 0.2, 0.8, 0.3, 0.4]

mean_value = sum(single_unit_data) / len(single_unit_data)
print("\nMean value of single-unit data:", mean_value)

# Detecting spikes (values above 0.7)
spikes = [x for x in single_unit_data if x > 0.7]
print("Detected spikes:", spikes)

# Topic 5: EEG data (Simulated Example)
import numpy as np

# Simulated EEG signal (sinusoidal signal)
time = np.linspace(0, 1, 500)  # 1 second at 500 Hz
frequency = 10  # 10 Hz
amplitude = np.sin(2 * np.pi * frequency * time)

plt.plot(time, amplitude)
plt.title('Simulated EEG Signal')
plt.xlabel('Time (s)')
plt.ylabel('Amplitude')
plt.show()
```
