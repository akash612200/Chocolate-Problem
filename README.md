# Chocolate-Problem
How Many Chocolates?
Description
Sanjay loves chocolates. He goes to a shop to buy his favourite chocolate. There he notices there is an offer going on, upon bringing 3 wrappers of the same chocolate, you will get new chocolate for free. If Sanjay has m Rupees. How many chocolates will he be able to eat if each chocolate costs c Rupees?

----------------------------------------------------------------------
Input:
Two positive integers m and c separated by a comma. The first integer is m and the second integer is c 

Output:
A single integer denoting the number of chocolates Sanjay was able to eat in total.

----------------------------------------------------------------------
Sample input:
15, 2

Sample output:
10

Explanation:
First, he will get 15/2=7 chocolates. He then will return 6 wrappers for 2 chocolates. And lastly, these two wrappers and the one he previously had will get him one more chocolate, making a total of 7+2+1=10 chocolates.

----------------------------------------------------------------------
Sample input:
3,1

Sample output:
4
# Anwer to this question 

my = input()
mylist = my.split(',')
m = int(mylist[0])
c = int(mylist[1])
choc = m//c
w = m//c
while(w//3 != 0):
    choc = choc + w//3
    w = w//3 + w%3 
print(choc)
