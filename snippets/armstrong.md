---
title: Armstrong
tags: Math
expertise: intermediate
author: EktaGujar
firstSeen: 2022-08-13T05:00:00-04:00
lastUpdated: 2022-09-15T19:27:53-02:00
---


Checks if the given number is armstrong or not.


- The Armstrong number is the number in which the sum of each digit powered to the total number of digits is the same as the given number.
- Use while loop and length of a number to calculate armstrong of a number.


```py
def armstrong (num):
   order = len(str(num))
   sum = 0
   temp = num
   while temp > 0:
       digit = temp % 10
       sum += digit ** order
       temp //= 10
   if num == sum:
       return "yes"
   else:
       return "no"
```


```py
armstrong(153) #yes
armstrong(1984) #no
```
