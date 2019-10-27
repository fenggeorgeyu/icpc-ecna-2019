Problem E

Just Passing Through

Justin and Fred are taking a road trip, traveling from West to East across their state. They have a few Road Trip Rules:

They must have an awesome time!

The trip must begin somewhere along the Western edge of the state and finish somewhere along the Eastern edge of the state.

Each step in their trip must move them either directly East, diagonally Northeast, or diagonally Southeast.

They want to travel through exactly 𝑛 “passes” (defined below).

Due to Fred’s sensitivity to higher elevations, they wish to minimize the cumulative sum of elevations during the trip.

They must have an awesome time!

Because Justin and Fred are traveling Eastward, a “pass” is any location with strictly lower elevations to its East and West and strictly higher elevations to its North and South. Consider the elevation map shown in Figure 1. Undrivable locations (either due to water or stubborn insistence on staying in-state) are shown in black, while passes are shown as gray. Locations adjacent to the border or to undrivable locations are not eligible for considerations as passes.

![Figure 1: A sample elevation map](img-0001.png)

Input
The input begins with three integers 𝑟 𝑐 𝑛 representing the number of rows and columns in the representation of the state’s topography (3≤𝑟,𝑐≤500) and the exact number of passes to be crossed (0≤𝑛≤10). The next 𝑟 lines each contain 𝑐 elevation entries. Undrivable locations are represented by −1, and all other elevations are between 0 and 1000. There is guaranteed to be at least one drivable location on both the Eastern and Western borders.

Output
Output the sum of the elevations along the optimal path which satisfies the Road Trip Rules. If no such path exists, output impossible.

Sample Input 1	

    5 7 2
    -1 -1 2 5 4 3 1
    3 4 1 4 1 2 1
    3 4 5 5 3 4 5
    2 3 2 1 2 3 2
    -1 5 4 1 4 4 2

Sample Output 1

    14

Sample Input 2	

    4 3 1
    3 4 5
    2 4 2
    1 5 4
    1 1 1

Sample Output 2

    impossible
