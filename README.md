# Python-Tuples

Exercise 1 – Working with Tuple & List
A problem you are trying to solve has the following data elements: 3, 1, 4, 1, 5, 9, 2, 5, 3, and 6. Create a Python
script that stores the above data elements of your problem in a tuple variable named “tup1”. Next create
another tuple variable named “tup2” that has the values 7 and 8 repeated five times by using the
multiplication operator (*). Lastly, use the tuple concatenation method to create a new tuple named
“super_tup” that will have the contents of the tuples named “tup1” and “tup2”.
Expected output:
super tuple: (3, 1, 4, 1, 5, 9, 2, 5, 3, 6, 7, 8, 7, 8, 7, 8, 7, 8, 7, 8)
After printing this super tuple, print the unique numbers contained in the tuple (use the set function).

Exercise 2 – Common Values
Write a Python script that counts the number of common items between two lists named “list1” and “list2”.
Form the starter code below, check if each item in list1 also appears in list2 and keep track of the number
of common items using the variable named “cnt”.
Here is the code template:
Expected output:
Number of common items is: 5
Can you use the set operations to obtain the same result?

Exercise 3 – Geometric Mean
Suppose that you have a collection of n numbers: 𝒂𝟏, 𝒂𝟐, ⋯ , 𝒂𝒏. Formally, the arithmetic mean (=what we
usually refer to as simply the mean or average) and the geometric mean are computed by the following
formulas:
Arithmetic mean: (𝒂𝟏 + 𝒂𝟐 + ⋯ + 𝒂𝒏)/𝒏
Geometric mean: (𝒂𝟏 × 𝒂𝟐 × ⋯ × 𝒂𝒏)𝟏/𝒏
The geometric mean is often used in finance to determine the performance results of an investment or
portfolio. One example is to compute average growth rates using the geometric mean and is referred to as the
compounded annual growth rate. For example, consider a stock that grows by 10% in year one, declines by
20% in year two, and then grows by 30% in year three. Then, the geometric mean of the growth rate is
calculated as follows:
((1 + 0.1) × (1 − 0.2) × (1 + 0.3))
1
3 = (1.1 × 0.8 × 1.3)1/3 = 0.046,
that is, 4.6% annually.
Write a Python program that computes the geometric mean of 1.03, 0.9, 1.36, 1.23, 1.08, 1.12, 1.55, 1.06, 1.05
and 0.92, which are stored as a Python list variable named “growth_rates”. The first step is to multiply all
numbers in the list growth_rates and store the result in a variable named “mult”. You can use a for loop
statement to do this step. Alternatively, you can use functions provided by the math package or the NumPy
package. The next step is to raise the value of mult to the power of 1/n, where n is the number of items in the
list growth_rates. Lastly, round the resulting number to two decimal places and assign the result to a variable
named geo_mean.
Here is the code template:

Exercise 4 – Sorting Dictionaries
A problem you are trying to solve has one data structure named “dict1”:
Use a for loop statement to go through the keys in descending order in your dict1 dictionary. For each
iteration in your loop statement, print the key-value pairs in your dict1 dictionary (can you use any of the
statements like reversed(), sorted(), and dict1.keys() in your solution?)
Your script should provide console output as indicated in the sample output below:

Exercise 5
A problem you are trying to solve has a Python string named “lorem” that has been split word-by-word
using the string split() method with an argument sep = ' ' to create a new list named “lorem_words”, as seen
in the starter code below. You have been asked to do the following:
1. Search for the documentation of the string split() method. Then write a brief description of the
string split() method as Python comments. Your description must contain
a. what split does,
b. syntax of split,
c. what are the arguments and what they do.
Lastly, in your own words, explain how the variable lorem_words got its value after running the
first two lines of the starter code based on your description of the string split() method.
2. Create a new (empty) dictionary named “word_len”.
3. Use a for loop with a sorted() statement (ascending order) for your lorem_words list. Inside your
for loop statement, add key-value pairs to your dictionary word_len, using each word in the
lorem_words list as the dictionary key, and the dictionary value being the length of the word (=
number of characters).
4. Print word_len.
Starter Code:
lorem = 'ut enim ad minim veniam quis nostrud exercitation'
lorem_words = lorem.split()
print(lorem_words)

Exercise 6
When working with data sets, it is useful to be able to categorize, for instance, a list of words by their first
letters as a dictionary of lists, as outlined in our textbook (in section 3.1 under the “diet” section, in the
subsection named “Default values”, pages 63-64). Our textbook covers the dictionary setdefault() method,
which is a useful, dean and more efficient method to create default dictionaries from lists. You have been
asked to do the following:
1. Search for the documentation of the dictionary setdefault() method. Then write a brief description
of the dictionary setdefault() method as Python comments. Your description must contain (1) what
setdefault does, (2) syntax of setdefault, and (3) what are the arguments and what they do.
2. Identify from the textbook (in section 3.1 under the “dict” section, in the subsection named “Default
values”) the relevant setdefault() method that creates a list of words by their first letters as a dict of
lists.
3. Implement this method in the starter code below. The correct implementation of this technique
should result in the sample Python console output.
Starter Code:
Expected output:
dictA: {‘a’: [‘action’, ‘apple’], ‘t’: [‘table’, ‘tennis’, ‘trap’]}
