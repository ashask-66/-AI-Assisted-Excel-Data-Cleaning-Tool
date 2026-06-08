import pandas as pd
import matplotlib.pyplot as plt

# Student Data
data = {
    "Name": ["Asha", "Rahul", "Sneha", "Kiran"],
    "Marks": [85, 78, 92, 67]
}

# Create Table
df = pd.DataFrame(data)

# Display Data
print(df)

# Find Average
average = df["Marks"].mean()
print("Average Marks =", average)

# Create Bar Chart
plt.bar(df["Name"], df["Marks"])

# Chart Title
plt.title("Student Marks Visualization")

# Labels
plt.xlabel("Student Names")
plt.ylabel("Marks")

# Show Chart
plt.show()
