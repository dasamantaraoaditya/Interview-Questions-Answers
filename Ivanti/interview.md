# Ivanti

## Round 1
- Disadvantages of micro services
- How to debug any bug in production
- In microservices there are multiple servers which can be scaled horizontally based on cpu and memory consumption. Every day at a given time all the server of the same microservice fail becasue of out of memory exception. How do you solve the problem as quickly as possible.
- Sql querys on groupBy and pagination
- Indexing in sql
- Different types of indexings and why they are used

## Round 2
- Merg two sorted arrays https://leetcode.com/problems/merge-sorted-array/ 
```
  class Solution {
    public void merge(int[] nums1, int m, int[] nums2, int n) {
        int nums1counter = m-1, nums2counter = n-1, resultCounter = m+n-1;
        while(nums1counter>=0 && nums2counter>=0){
            if(nums1[nums1counter] < nums2[nums2counter]){
                nums1[resultCounter] = nums2[nums2counter];
                nums2counter--;
            }
            else{
                nums1[resultCounter] = nums1[nums1counter];
                nums1counter--;
            }
            resultCounter--;
        }
        while(nums2counter>=0){
            nums1[resultCounter] = nums2[nums2counter];
            nums2counter--;
            resultCounter--;
        }
    }
  }
  ```
  
- Different injection mechanisms in spring
  https://www.programmergirl.com/spring-dependency-injection/
  
- Different bean scopes in spring
  https://www.tutorialspoint.com/spring/spring_bean_scopes.htm
  
- How to instantitate single bean with different values/instances
  By using @qualifier https://gateway.zscalertwo.net/auD?origurl=https%3A%2F%2Fwww%2ebaeldung%2ecom%2fspring%2dqualifier%2dannotation&_ordtok=D0k3WV5QDQL5FWktQq22z526r4 
