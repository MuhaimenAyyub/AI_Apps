# BMI Calculator

```py
def calculate_bmi(weight, height):
    calculation = weight / (height * height)
    return calculation

def show_results(weight, height):
    calculate = calculate_bmi(weight, height)
    if calculate <=18.5:
        print("Underweight")
    elif calculate > 18.5 and calculate <=25:
        print("Normal")
    else:
        print("Overweight")

people = int(input('Enter number of people'))
for i in range(people):
    # The above code will run depending on the number of people you add
    weight = float(input("Enter weight: "))
    height = float(input("Enter height: "))
    show_results(weight, height)
    ```