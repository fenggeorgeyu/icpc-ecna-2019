Problem C

Cheese, If You Please

The “We Cut The Cheese” specialty food store sells specialized blendings of cheeses. For example, their Italian Blend is made up of 50% provolone, 30% mozzarella and 20% parmesan, while their African Safari is made up of 74% domiati, 25% areesh with just a hint (1%) of bokmakiri. You started working at the store as a cheese blend taster, but two years and 45 pounds later you have worked your way up to head of the accounting office. Every week the store gets various shipments of cheeses, depending on the time of year, market price and other factors. Given these amounts and the percentages required for each cheese blend, you are asked every week to determine the optimal use of these cheeses to maximize profit. When the store just made a few different cheese blends this could be done by hand, but with business expanding faster than a cheese souffle, the number of blends has also grown to the point where a program is now needed to determine the optimal use of the cheese shipments. So the question is: Are you gouda-nough to write such a program?

Input
Input starts with a line containing two positive integers 𝑛 𝑚 (1≤𝑛,𝑚≤50), where 𝑛 is the number of types of cheese used to make the cheese blends and 𝑚 is the number of different cheese blends offered by the store. The next line contains 𝑛 integers 𝑤1 𝑤2 … 𝑤𝑛 (0≤𝑤𝑖≤500), where 𝑤𝑖 is the number of pounds of cheese type 𝑖 that the store has on-hand. Following this are 𝑚 lines of the form 𝑝1 𝑝2 𝑝3 … 𝑝𝑛 𝑡 (0.0≤𝑝𝑖≤100.0, 0.0≤𝑡≤10.0), where 𝑝𝑖 indicates the percentage of cheese 𝑖 found in the blend, and 𝑡 is the profit per pound for the blend. Percentages are given with one decimal place, profits are given with two decimal places.


Output
Output the maximum profit that can be obtained for the given pounds of cheese, blending percentages and profits, assuming all of the blended cheeses get sold. Round your answer to the nearest penny.


Sample Input 1

    3 2
    100 150 100
    50.0 50.0 0.0 3.20
    0.0 50.0 50.0 2.80

Sample Output 1

    920.00

Sample Input 2

    3 2
    100 150 100
    50.0 50.0 0.0 3.20
    0.0 40.0 60.0 2.80

Sample Output 2

    1000.00



