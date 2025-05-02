# Mean-Variance-Standard Deviation Calculator

This project is a Python function that leverages NumPy to calculate several statistical metrics — **mean**, **variance**, **standard deviation**, **max**, **min**, and **sum** — across **rows**, **columns**, and the **flattened array** of a 3x3 matrix.

## 📌 Features
- Accepts a list of exactly **9 numeric values**
- Converts the list to a 3x3 NumPy array
- Calculates metrics along:
  - Axis 0 (columns)
  - Axis 1 (rows)
  - Flattened matrix (entire array)
- Returns a dictionary with all the calculated values
- Raises an error if the list has fewer or more than 9 elements

## 📦 Example

```python
from calculator import calculate

result = calculate([0, 1, 2, 3, 4, 5, 6, 7, 8])
print(result)
Sample Output:
python
Copy
Edit
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.666..., 0.666..., 0.666...], 6.666...],
  'standard deviation': [[2.44..., 2.44..., 2.44...], [0.81..., 0.81..., 0.81...], 2.58...],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
⚠️ Error Handling
If the input list does not contain exactly 9 elements, the function will raise:

makefile
Copy
Edit
ValueError: List must contain nine numbers.
📁 Files
calculator.py: Contains the calculate() function

📚 Requirements
Python 3

NumPy
