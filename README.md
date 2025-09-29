# BMI-Calculator
A modular Python function that calculates Body Mass Index (BMI) with input validation, health categorization, and educational context. Built using an incremental development approach to showcase clear logic, robust testing, and user-centered design
```python
def BMI(height, mass):
    """
    Calculates Body Mass Index (BMI) based on height (m) and mass (kg).
    Returns BMI value and health category with a disclaimer.
    """
    if height <= 0 or mass <= 0:
        return "Invalid input: height and mass must be positive numbers."
    bmi = mass / (height ** 2)
    if bmi < 18.5:
        category = "Underweight"
    elif bmi < 25:
        category = "Normal weight"
    elif bmi < 30:
        category = "Overweight"
    else:
        category = "Obese"
    return f"BMI: {bmi:.2f} ({category})\nNote: BMI is a general guideline."
```
