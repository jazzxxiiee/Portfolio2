# Portfolio2
## Title: University Student Risk Assessment System
### Name: Jabez Dan Lloyd O. Llanera - BS Chemical Engineering 1A

```python
print("===== UNIVERSITY STUDENT RISK ASSESSMENT =====\n")
```
### User Input
```python
name = input("Enter student name: ")
attendance = float(input("Enter attendance percentage: "))
quiz_average = float(input("Enter quiz average: "))
violations = int(input("Enter number of violations: "))
```
### Conditional Statements
```python
if attendance >= 90 and quiz_average >= 90 and violations == 0:
    status = "ACADEMIC EXCELLENCE"
    action = "Eligible for recognition"

elif attendance >= 80 and quiz_average >= 75 and violations <= 2:
    status = "SAFE STATUS"
    action = "No intervention needed"

elif attendance >= 70 and quiz_average >= 70 and violations <= 4:
    status = "WARNING STATUS"
    action = "Guidance counseling required"

elif attendance >= 60 or quiz_average < 70 or violations >= 5:
    status = "CRITICAL STATUS"
    action = "Parent conference required"

else:
    status = "DEAN'S INTERVENTION"
    action = "Subject for disciplinary review"
```
### Output
```python
print("\n========== ASSESSMENT RESULT ==========")
print("Student Name   :", name)
print("Attendance     :", attendance, "%")
print("Quiz Average   :", quiz_average)
print("Violations     :", violations)
print("Status         :", status)
print("Recommended Action :", action)
print("=======================================")

print("\nProgram Finished Successfully!")
```
