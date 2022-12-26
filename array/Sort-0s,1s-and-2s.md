# Sort an array of 0s, 1s and 2s 
## Given an array A[] consisting of only 0s, 1s, and 2s. The task is to write a function that sorts the given array. The functions should put all 0s first, then all 1s and all 2s in last. 
## This problem is also the same as the famous “Dutch National Flag problem”. 
 
Input: {0, 1, 1, 0, 1, 2, 1, 2, 0, 0, 0, 1}
Output: {0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 2, 2} 

[Poblem Link](https://practice.geeksforgeeks.org/problems/sort-an-array-of-0s-1s-and-2s4231/1?utm_source=gfg&utm_medium=article&utm_campaign=bottom_sticky_on_article)
 
#### Efficient Solutin 
Time Complexity:- O(N) , Space Complexity:- O(1)
~~~
void sort012(int a[], int n)
    {
        
        int count=0;
        for(int i=0; i<n; i++)
        {
            if(a[i]==0)
            {
                swap(a[i],a[count]);
                count++;
            }
        }
        
        int count1=0;
        count1=count;
        for(int i=count; i<n; i++)
        {
            if(a[i]==1)
            {
                swap(a[i],a[count1]);
                count1++;
            }
        }
        
    }
    
