# Exercise: Array DataStructure

1. Let us say your expense for every month are listed below,
	1. January -  2200
 	2. February - 2350
    3. March - 2600
    4. April - 2130
    5. May - 2190

Create a list to store these monthly expenses and using that find out,

    1. In Feb, how many dollars you spent extra compare to January?
    2. Find out your total expense in first quarter (first three months) of the year.
    3. Find out if you spent exactly 2000 dollars in any month
    4. June month just finished and your expense is 1980 dollar. Add this item to our monthly expense list
    5. You returned an item that you bought in a month of April and
    got a refund of 200$. Make a correction to your monthly expense list
    based on this
    
[MY SOLUTION]
monthly_expenses = [2200, 2350, 2600, 2130, 2190]

1. extra_feb_jan = monthly_expenses[1] - monthly_expenses[0]
2. total_expense_q1 = 0
   for i in range(3):
   	total_expense_q1 += monthly_expenses[i]
3. for i in range(len(monthly_expenses)):
   	if monthly_expenses[i] == 2000:
		print("You did")
4. monthly_expenses.append(1980)
5. monthly_expenses[3] = monthly_expenses[3] - 200
		


[Solution](https://github.com/codebasics/data-structures-algorithms-python/blob/master/data_structures/2_Arrays/Solution/1_expenses.py)

2. You have a list of your favourite marvel super heros.
```
heros=['spider man','thor','hulk','iron man','captain america']
```

Using this find out,

    1. Length of the list
    print("The length of the list is", len(heros))
    2. Add 'black panther' at the end of this list
    heros.append('black panther')
    3. You realize that you need to add 'black panther' after 'hulk',
       so remove it from the list first and then add it after 'hulk'
    heros.remove('black panther')
    heros.insert(3, 'black panther')
    4. Now you don't like thor and hulk because they get angry easily :)
       So you want to remove thor and hulk from list and replace them with doctor strange (because he is cool).
       Do that with one line of code.
    heros = ['spider man','doctor strange','doctor strange','iron man','captain america']
    heros[1:3] = 'doctor strange'
    5. Sort the heros list in alphabetical order (Hint. Use dir() functions to list down all functions available in list)
    heros.sort()

[Solution](https://github.com/codebasics/data-structures-algorithms-python/blob/master/data_structures/2_Arrays/Solution/2_marvel.py)


3. Create a list of all odd numbers between 1 and a max number.
Max number is something you need to take from a user using input() function
max_number = int(input("Please provide a positive number greater than 1: "))
odd_lst = []
for i in range(1, max_number):
	if i%2:
		odd_lst.append(i)
[Solution](https://github.com/codebasics/data-structures-algorithms-python/blob/master/data_structures/2_Arrays/Solution/3_odd_even_numbers.py)

