Problem J

Taxed Editor

Reed Dacht is a freelance book editor who works out of his home. Various publishers send him texts to read along with a deadline date for when they would like his editorial comments to be sent back to them. Reed is very precise with his reading and will never read more than one book at a time, so he never starts a new book until after he is finished reading the previous one. He is willing to change the rate (number of pages per day) at which he reads books, but to be fair to each of his clients he insists on using the same speed for all books.

The other day Reed got a large set of editing requests and has a bit of a problem. He doesn’t think that there’s any way he can read all of the books by the specified deadlines. He could set his reading speed high enough to get them all done in time, but that might compromise the accuracy of his editing (as well as severely tax his eyesight). To avoid that he could select a slower reading speed, but then too many of the editing jobs would go past their deadlines. He has decided on a compromise: he is willing to let a small number of books go past deadline (so as to annoy only a small number of clients) and will set his reading speed to the smallest possible number of pages per day so that no more than that number of books will be late. But what should that reading speed be? That’s where you come in.

Input

Input starts with two integers 𝑛 𝑚 where 𝑛 (1≤𝑛≤105) is the number of books to edit and 𝑚 (0≤𝑚<𝑛) is the number of editing jobs that Reed will allow to be late. Following this are 𝑛 lines each describing one book. Each line contains two integers 𝑙 𝑑 where 𝑙 (1≤𝑙≤109) is the length (in pages) of the book and 𝑑 (1≤𝑑≤104) is the deadline for that book (number of days until is it due).

Output

Output the minimum integer speed (pages per day) which allows no more than 𝑚 late editing jobs.

Sample Input 1	

    3 1
    450 9
    500 6
    300 4

Sample Output 1

    84
