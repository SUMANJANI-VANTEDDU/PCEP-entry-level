#Objectives#

using the if-elif-else statement;

Scenario
As you surely know, due to some astronomical reasons, years may be leap or common. The former are 366 days long, while the latter are 365 days long.

Since the introduction of the Gregorian calendar (in 1582), the following rule is used to determine the kind of year:

if the year number isn't divisible by four, it's a common year;
otherwise, if the year number isn't divisible by 100, it's a leap year;
otherwise, if the year number isn't divisible by 400, it's a common year;
otherwise, it's a leap year.

It would be good to verify if the entered year falls into the Gregorian era, and output a warning otherwise: Not within the Gregorian calendar period. 
Tip: use the != and % operators.









```
year = int(input("Enter a year: "))
if year<1582:
    print("not within the Gregorian calendar")
    exit()
elif year%4!=0:
    print("common year")
    exit()
elif year%100!=0:
    print("Leap year")
    exit()
elif year%400!=0:
    print("common year")
    exit()
else:
    print("Leap year")
```
