# python-activity-based-learing-1
Algorithm
1.Start.
2.Enter water consumption for 3 households.
3.Calculate bill using slabs:
First 100 units: ₹2/unit
Above 100 units: ₹4/unit
4.Add fixed fee ₹50.
5.if consumption exceeds 200 units, add ₹100 penalty.
6.Display bills and identify excessive usage.
7.Stop.
flowchart
Start
Input household units
Calculate slab bill + fee + penalty
Check usage above 200 units
Display bills and usage
Stop
units = [80, 150, 250]

for i in range(3):
    u = units[i]

    if u <= 100:
        bill = u * 2
    else:
        bill = 200 + (u - 100) * 4

    bill += 50

    if u > 200:
        bill += 100

    print("Household", i + 1, "Bill: Rs.", bill)

    if u > 200:
        print("Excessive usage!")
Household 1 Bill: Rs. 210
Household 2 Bill: Rs. 450
Household 3 Bill: Rs. 850
Excessive usage!


