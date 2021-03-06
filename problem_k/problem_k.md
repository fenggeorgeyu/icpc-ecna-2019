
Problem K

Where Have You Bin?

Ben Bean owns Ben Bean’s Bin Bonanza which offers storage bins to the five big companies in town: a rubber band company, a Mercedes Benz dealership, a bing cherry farm, a bonbon candy store and a bun bakery. Together they store their bands, Benzes, bings, bonbons and buns in Ben’s bins.

Ben has 𝑛 bins altogether arranged in a single row, numbered 1 to 𝑛. While not all of the bins may be in use at any given time, Ben finds it useful to keep all the bins for one company contiguous. Thus, when a company needs a new bin or relinquishes one it no longer needs, Ben may need to move items from one bin to another to make sure all of that company’s bins stay next to each other. Sometimes Ben has a choice of which bin to move, so he has assigned a cost to each bin equal to the number of items stored in the bin (removing items from a relinquished bin and/or moving items into a new bin are the company’s responsibility and do not add to Ben’s costs). Obviously when moving bins Ben wants to keep the cost as low as possible.

If a single company has to make changes Ben can usually figure out the cheapest way to move items around, but typically at the end of each business quarter all of the five companies will make additions and deletions of bins as they reassess their product lines. In cases like this, deciding the lowest-cost set of moves is more difficult. Consider the situation in Figure 1a which shows 6 bins storing items from the five companies labeled A, E, I, O and U. The numbers in parentheses indicate the number of items in that bin (and thus the cost of moving the items from that bin to another). Suppose that at the end of the quarter company U decides it no longer needs bin 6 and company A requests a second bin. One possibility is to move E’s items from bin 2 to the empty bin 6 which frees up bin 2 for company A (Figure 1b)—the cost of this rearrangement to Ben is 4. The optimal move though is to move U’s items from bin 5 to bin 1 and move A’s items from bin 1 to bin 5 and giving company A bin 6 (Figure 1c)—the cost of this move is 3. Ben could also have moved A’s items from bin 1 to bin 6 to achieve the same optimal cost. Notice that in all cases removing the three items from U’s bin 6 and adding the seven items to A’s second bin does not cost anything to Ben.

![Figure 1: Sample Input 1.](img-0001.png)

Input

Input starts with a string of characters of length 𝑛 (1≤𝑛≤150) indicating the initial usage of the bins. The characters will all be from the set {A, E, I, O, U, X} indicating either the company using the bin or an empty bin (X). Following this is a row of 𝑛 integers indicating the number of items in each bin; values at locations corresponding to an empty bin will always be 0 and values at locations corresponding to a company’s bin will be positive and ≤100. Bins for any one company will always be contiguous.

The next line starts with an integer 𝑑 (0≤𝑑≤𝑛) indicating the number of deletions for this quarter. Following this are 𝑑 integers. Each integer specifies a bin which is no longer needed by a company. None will ever correspond to an already empty bin. On the final line is a positive-length string of characters indicating the new bins requested. If this string is a single X then no new bins are being requested. Otherwise the characters will all be in the set {A, E, I, O, U}, in no particular order, each character representing a request for a new bin by the corresponding company. There will always be enough bins to handle any set of changes.

Output

Output the minimal cost required to satisfy all the bin changes while keeping each company’s bins contiguous.

Sample Input 1	

    AEIOUU
    1 4 6 9 2 3
    1 6
    A

Sample Output 1

    3

Sample Input 2	

    AEIOUU
    10 4 6 9 2 3
    1 6
    A

Sample Output 2

    4

Sample Input 3	

    AEIOUU
    1 4 6 9 2 3
    4 5 1 4 3
    EUE

Sample Output 3

    0


