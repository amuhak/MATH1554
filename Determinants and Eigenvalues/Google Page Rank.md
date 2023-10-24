![[Google Page Rank.png]]

![[Google Page Rank-1.png]]

![[Google Page Rank-2.png]]

If we have:
![[Google Page Rank-3.png|400]]
P will be: 
![[Google Page Rank-4.png|400]]

# Problem 
- We do not have a unique unique steady-state for all pages
- pages that do not link to other pages can have the largest importance, or highest PageRank
# Fix
- If a user reaches a page that does not link to other pages, the user will choose any page in the web, with equal probability, and move to that page.
- Corresponding fixed matrix:
![[Google Page Rank-5.png|400]]
![[Google Page Rank-6.png|500]]
> [!WHY THIS WORKS]
> This works because we are taking each column and reducing its sum by $(1-p)$. Then we are adding $(1-p)$ back to the column, but evenly distributed over the whole column. This insures that the sum of the column of the final matrix stays $= 1$.

