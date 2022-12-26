# Segregate 0s and 1s in an array 
## You are given an array of 0s and 1s in random order. Segregate 0s on left side and 1s on right side of the array [Basically you have to sort the array]. Traverse array only once. 
Input array   =  [0, 1, 0, 1, 0, 0, 1, 1, 1, 0] 
Output array =  [0, 0, 0, 0, 0, 1, 1, 1, 1, 1] 

[Problem Link](https://practice.geeksforgeeks.org/problems/segregate-0s-and-1s5106/1?utm_source=gfg&utm_medium=article&utm_campaign=bottom_sticky_on_article)
 
#### Efficient Solution 
Time Complexity:- O(N) , Space Complexity:- O(1)
~~~
void segregate0and1(int arr[], int n) {
        
        int count=0;
        for(int i=0 ;i<n; i++)
        {
            if(arr[i]==0)
           { swap(arr[i],arr[count]);
           count++;}
        }
    }
~~~~


