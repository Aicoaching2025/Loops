# 📊 Insurance Cost Comparison

This project visualizes and compares estimated vs actual insurance costs for a set of individuals using Python and Matplotlib.

## 📌 Features
- Calculates average insurance cost
- Compares estimated and actual costs using a bar chart
- Highlights whether actual costs are above or below average
- Provides an updated estimate with a 10% increase

## 🛠️ Technologies Used
- Python 🐍
- Matplotlib 📊
- NumPy 🔢

## 🚀 Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/insurance-cost-comparison.git
   cd insurance-cost-comparison
   ```
2. Install dependencies:
   ```sh
   pip install matplotlib numpy
   ```
3. Run the script:
   ```sh
   python insurance_cost_analysis.py
   ```

## 📈 Visualization
The script generates the following bar chart comparing estimated vs actual insurance costs:

![Insurance Cost Comparison](https://via.placeholder.com/800x400?text=Chart+Preview)

## 📝 Code Overview
```python
import matplotlib.pyplot as plt
import numpy as np

names = ["Judith", "Abel", "Tyson", "Martha", "Beverley", "David", "Anabel"]
estimated_insurance_costs = [1000.0, 2000.0, 3000.0, 4000.0, 5000.0, 6000.0, 7000.0]
actual_insurance_costs = [1100.0, 2200.0, 3300.0, 4400.0, 5500.0, 6600.0, 7700.0]

average_cost = sum(actual_insurance_costs) / len(actual_insurance_costs)
x = np.arange(len(names))

fig, ax = plt.subplots(figsize=(10, 6))
ax.bar(x - 0.2, estimated_insurance_costs, width=0.4, label='Estimated Costs', alpha=0.7)
ax.bar(x + 0.2, actual_insurance_costs, width=0.4, label='Actual Costs', alpha=0.7)
ax.axhline(y=average_cost, color='red', linestyle='--', label=f'Average Cost: ${average_cost:.2f}')
ax.set_xticks(x)
ax.set_xticklabels(names)
ax.set_xlabel("Individuals")
ax.set_ylabel("Insurance Costs ($)")
ax.set_title("Comparison of Estimated vs Actual Insurance Costs")
ax.legend()
plt.xticks(rotation=45)
plt.show()
```

## 📬 Contact
For questions, feel free to reach out:
- 📧 Email: aicoaching20215@gmail.com


### ⭐ If you found this useful, please consider giving a star on GitHub! 🚀


