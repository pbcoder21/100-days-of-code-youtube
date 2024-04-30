# Excersice 2: Good Morning Sir
Create a python program capable of greeting you with Good Morning, Good Afternoon and Good Evening. Your program should use time module to get the current hour. Here is a sample program and documentation link for you:
```python
import time
timestamp = time.strftime('%H:%M:%S')
print(timestamp)
timestamp = time.strftime('%H')
print(timestamp)
timestamp = time.strftime('%M')
print(timestamp)
timestamp = time.strftime('%S')
print(timestamp)
# https://docs.python.org/3/library/time.html#time.strftime
```
## [Next Lesson>>](https://replit.com/@codewithharry/16-Day-16-Match-Case)

Solution: 
```python
import time
timestamp = time.strftime('%H:%M:%S')
print("The time right now is",timestamp)
hours = int(time.strftime('%H'))
if hours >= 0 and hours <= 12:
    print("Good Morning Captain")
elif hours > 12 and hours < 17:
    print("Good Aternoon Captain")
elif hours > 17 and hours < 20:
    print("Good Evening Captain")
else:
    print("Good Night")
```
