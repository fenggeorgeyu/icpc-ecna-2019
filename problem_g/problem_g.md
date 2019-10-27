
Problem G

Out of Sorts

Ann Logan is fascinated with finite sequences of integers. She is particularly interested in sequences of the form 𝑥1,𝑥2,…,𝑥𝑛 where:

𝑥𝑖=(𝑎𝑥𝑖−1+𝑐)mod𝑚,

𝑛, 𝑚, 𝑎, and 𝑐 are positive integer constants,

𝑥0 is a non-negative integer constant, and

all 𝑛 values are unique.

For example, if 𝑛=5, 𝑚=8, 𝑎=1, 𝑐=3, and 𝑥0=3, the sequence is 6, 1, 4, 7, 2 (𝑥1=(1⋅3+3)mod8=6, 𝑥2=(1⋅6+3)mod8=1, and so on). Note that she does not consider the initial value 𝑥0 to be part of the sequence.

Ann wants to be able to quickly determine, for any integer value, whether or not it appears within a finite sequence of this form. Given values of 𝑛, 𝑚, 𝑎, 𝑐, and 𝑥0, she plans to follow this list of steps:

Generate the sequence 𝑥1,⋯,𝑥𝑛 and store it in an array.

Sort the array.

Perform a binary search of the array for each integer of interest to her.

Ann’s search algorithm, while not the most efficient possible, is pretty straightforward and understandable to anyone familiar with binary search: after calculating the midpoint mid at each step of the calculation (using mid = (low+high)/2), she first checks whether or not the value at location mid is equal to the search value x. If not, she then narrows the search according to whether x is strictly less than or strictly greater than the value at location mid.

Unfortunately, Ann is absent-minded and she lost her list of steps. She managed to remember the first and last step, but …she forgot to sort the array before performing her binary search! Needless to say, this means that many values that are in the (unsorted) array will not be found by a binary search, although surprisingly some can. In the example above, both 4 and 7 can be found with Ann’s binary search. How many values can be found for various sequences? Don’t botch it up!

Input

Input consists of a line containing five integers 𝑛, 𝑚, 𝑎, 𝑐, and 𝑥0 (1≤𝑛≤106, 1≤𝑚,𝑎,𝑐≤231−1, 0≤𝑥0≤231−1), where 𝑛 is the length of the sequence 𝑥1,…,𝑥𝑛 to be generated and 𝑚, 𝑎, 𝑐, and 𝑥0 are the constants used for generating the sequence. All values in the generated sequence are guaranteed to be unique.

Output

Output the number of sequence values that could be found using Ann’s version of binary search, assuming she forgot to sort the sequence.

Sample Input 1	
    
    5 8 1 3 3

Sample Output 1

    2

Sample Input 2	

    6 10 1234567891 1 1234567890

Sample Output 2
    
    6
