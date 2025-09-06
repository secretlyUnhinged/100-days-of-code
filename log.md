# 100 Days Of Code - Log

### Day 1: August 9,2025(Saturday)

**Today's Progress**: Started the shorter graph series for revision(by takeuforward). Revised basics of graph,bfs,dfs,intuition behind rotten oranges problem. 

**Thoughts:** Have been tinkering around with codeforces round 1037(div 3) problems A,B,C. Solved A on the first attempt with optimal time complexity solution but struggled with B and C.


### Day 2: August 10,2025(Sunday)

**Today's Progress**: Solved rotten oranges, number of provinces, number of islands,flood fill.

**Thoughts:** Hopefully will wrap up graphs by end of this week and move on to trees. Tweaked the recursion function i am "supposed" to use and saw how it affected the whole code, then added necessary conditions to make up for the "missing" argument, instead of blindly accepting the function template.


### Day 3: August 11,2025(Monday)

**Today's Progress**: Revised graph cycle detection algorithm using bfs/dfs and bipartite graph using bfs.

**Thoughts:** 
**Link(s) to work**

### Day 4: August 13,2025(Tuesday)

**Today's Progress**: Revised topological sort using dfs/bfs.
**Link(s) to work**

### Day 5: August 15,2025(Thursday)

**Today's Progress**: Did a data science case study project based on clustering for a consultancy startup.
**Thoughts:** Dataset was full of unknown values, to the point that imputation or removal was not possible, hence I created a separate class for it so that it won't lead to noisy clusters. Maybe I could have used inference-based Bayesian formula or decision tree to find the most probable value but it was MNAR. Further investigation could be done to find if there is a pattern to the missingness.
**Link(s) to work**

### Day 6: August 16,2025(Friday)

**Today's Progress**: worked on the clustering project some more, used cramers v, silhouette core, Davies–Bouldin Index (DBI) and mca to finally plot the clusters.
**Thoughts:** number of outliers were more but in mca plot, they were compressed as the feature space was 5d but mca is 2d plot. learnt how to find the features that are more important compared to the rest using statistical methods.
**Link(s) to work**


### Day 7: August 23,2025(Saturday)

**Today's Progress**: Deep copy of a graph,find the minimum area to cover all ones II(3197)
**Thoughts:** used dfs+hashmap to create a deep copy of a graph. while using dfs,infinite recursion is always a possibility.
**Link(s) to work**

### Day 8: August 24,2025(Sunday)

**Today's Progress**: finished find min area to cover all ones II, longest subarray of ones after deleting one elt(1493)
**Thoughts:** look at other approaches to min area problem(i did brute force i think?), uses sliding window+2 pointer ,found a dsa pattern flowchart. For the min area II propblem, maybe concept of disjoint sets could be used?(need to look into it further)
**Link(s) to work**

### Day 9: August 25,2025(Monday)

**Today's Progress**: diagonal traversal lc, looked into albumentations for an open source contribution to off, learnt about medclip architecture
**Thoughts:** d=r+c and odd diag vs even diag, need to find more suitable open source issues in ml
**Link(s) to work**

### Day 10: August 26,2025(Tuesday)

**Today's Progress**: search a 2d matrix lc
**Thoughts:** flattened and performed binary search.
**Link(s) to work**

### Day 11: August 27,2025(Wednesday)

**Today's Progress**: count inversions gfg, reverse pairs, revised mergesort

**Thoughts:** count inversion uses merge sort but before the merging step, count the number of inversions using mid-left+1 and return that(so the change is made in merge step). In reverse pairs, we use merge sort again but there is an additional function right before merging and after sorting countpairs(it keeps the cnt variable and updates cnt+=right-(mid+1))
**Link(s) to work**

### Day 12: August 28,2025(Thursday)

**Today's Progress**: defuse the bomb lc, count substr that satisfy k constraint lc , substr of size 3 with distinct char lc, Longest Nice Substring lc, find the k beauty of a number lc

**Thoughts:** did the brute force approach first, then saw how sliding window could optimize it(we duplicate the array because it is a circular array so wrap around is easy and no negative indices). brute force for second problem is o(n3), prefix array o(n2) and sliding window is o(n). for the third problem, simple sliding window of fixed size and checking for duplicates. nice substring problem uses recursion + hashSet to divide the string at i and check recursively. for k beauty of number problem, we use sliding window, convert nums to string then the substrings back to nums to find out if it is a divisor of the string.
**Link(s) to work**

### Day 11: August 29,2025(Friday)

**Today's Progress**: minimum ecolors to get consecutive black blocks lc, max length substring with 2 occurences lc, longest harmonious subsequence lc, alternating groups I lc, find x sum of all k long subarrays I lc,

**Thoughts:** uses sliding window and counts the number of whites in each window(min no is ans). second problem uses frequency map+ sliding window(freq map is used to keep the count of the char, then window slides based on the condition of freq). third problem uses frequency map( hashmap keep count of all elts of the array, then checks if i+1 element exists, if it does then it adds the freq count of i and freq count of i+1, maxlen variable keeps count of max such sum, methods like freq.keySet(), freq.containsKey(), freq.getOrDefault(num,0)); check out the tw pointer approach for this problem. for alternating groups problem: used sliding window on circular array(either modulo or duplicate and extend the array). uses sliding window+ freq map for each window sorted in desc order of freq first then value or sliding window+ heap(priority queue).

**Link(s) to work**

### Day 12: August 30,2025(Saturday)

**Today's Progress**: Contains Duplicate II, max avg subarray I

**Thoughts:** uses hashSet to keep track in the window+ sliding window(remove i-k elt if window size>k). second problem just uses sliding window(compute first k sum then slide the window, find max sum then return avg of max sum).
**Link(s) to work**

### Day 13: August 31,2025(Sunday)

**Today's Progress**: maximum subarray with equal products, did linux commands

**Thoughts:** one thing to look out for is the max lcm possible. looked into 2 different solutions, more about number theory than code. need to do more linux. Did a bunch of leetcode (not so) easy questions on sliding window, next probably will do binary search, mixing it up with sliding window medium level questions.

**Link(s) to work**https://github.com/MaheshShukla1/Linux-Basics-to-Advanced-Complete-Commands-Scripting-System-Administration-Guide/wiki/Linux%E2%80%90cheatsheet

### Day 14: September 2,2025(Tuesday)

**Today's Progress**: divisor game lc


### Day 15: September 3,2025(Wednesday)

**Today's Progress**:counting bits lc, min cost climbing stairs lc

**Thoughts:** for counting all ways type of problem, recursion is used then we can apply memoization and later, tabulation.


### Day 16: September 4,2025(Thursday)

**Today's Progress**: combination sum iv lc, frog jump gfg, frog jump with k distance(follow up of frog jump gfg), maximum sum without adjacent elememts gfg/house robber lc, house robber II lc/house robber circular gfg

**Thoughts:** this can be done using recursion, recursion+dp or dp(tabulation): in dp approach, we create a dp array from 0 to target, it tells how many ways there are to reach target. dp[0]=1 because the only way to get 0 is choosing no num as all num elts>0, then we loop through num array and calculate the dp array for i to target and it is formed by i-nums[j],(dp[i]+=dp[i-nums[j]). frog jump gfg did using recursion+memoization, thenn tabulation. **there are rules to convert recursion to memoization and rules to write aany recursion.Rules for recursion: 1. write in terms of index  2. do all stuffs to the index  3. return min, max, or sum of step 2.  Rules to convert recursion to memoization: 1. declare dp array of n+1  2. then before returning store it in the dp array  3. check if dp[index]!=1 then return dp[index].** the frog jump in gfg is different from frog jump in lc, in gfg, we can jump only 1 or 2 units and we are supposed to reach the last elt of  the array and the cost of each jump is abs difference between the idx and idx-1 or idx-2. for the follow up questions, we run a for loop upto k and calculate the jumps(jump=f(idx-j)+abs(arr[idx]-arr[idx-j]), consider minsteps as min(jump, minSteps). for max sum w/o adj elts, i used recursion first then recursion+memoization, then tabulation, one thing to note is that for tabulation you have to add an edge case for neg index for pick elt. finally return dp[n-1] where dp[i]=max(pick,npick) as we have the option to either pick an elts or not pick an elt.

### Day 17: September 5,2025(Friday)

**Today's Progress**: ninja's training 2d dp, max depth of a tree lc, binary balanced tree lc, diameter of binary tree lc

**Thoughts:** we take day and last as the index, last is the last task perform, then we find that day=0 is the base case and then we can use recursion+memoization. for tabulation, check out the base case, in this problem we have four cases as day=0 but the task value can be 0,1,2,3 so dp[0][0],dp[0][1], so on. max depth of tree can be done using level order traversal or recursion, i used recursion where we traverse the left subtree and right subtree, then the depth is 1+max(left_height,right_height). for the binary balanced tree, we used the same concept of findin left and right height by recursion but we check if abs difference >1, if yes return -1 else return depth, then -1 is false else true. for the diameter of binary tree, we need max distance between any two nodes, so we use the same concept of left height and right height by recursion but we use an array called diam of size 1 to store the max diam per iteration(using a var instead of array doesnt work as we need to pass by reference not value), then we do diam[0]=max(diam[0],left_height+right_height) and return the depth as usual(1+max(left_height,right_height).


### Day 18: September 6,2025(Saturday)

**Today's Progress**:max path sum of binary trees lc, same tree lc

**Thoughts:** use the concept of max height(recursion) and store sum of left subtree + right subtree + node val and track max left sum right sum. second ques, do any traversal at the same time and check if they match.




