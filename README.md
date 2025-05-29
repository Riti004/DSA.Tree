# DSA.Tree
#102. Binary Tree Level Order Traversal
Given the root of a binary tree, return the level order traversal of its nodes' values. (i.e., from left to right, level by level).


   1.creact a vector that stors another vector.
       vector<vector<int>>ans;
   2.creact a queue.
   3.push the root into the queue
   4.while queue is not empty
      ->find the size of the queue
      -> make another vector<int>level
      ->traverse the queue and pop the front 
         TreeNode* temp=q.front();
                q.pop();
      ->check if the left and right of temp exists if it does push them to vector<int>level
      ->push level inside ans 
    5. return ans 
![image](https://github.com/user-attachments/assets/d87ae3d6-5b99-4b9f-b777-194a6abb419b)
