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


#104. Maximum Depth of Binary Tree
Given the root of a binary tree, return its maximum depth.
A binary tree's maximum depth is the number of nodes along the longest path from the root node down to the farthest leaf node.

   1.if the node is NULL, it returns 0
   2.when present in a node do +1 for the present node 
   3.tarverse to the left and traverse to the right and find the depth of the subtrees recursively
       int left=maxDepth(root->left);
        int right=maxDepth(root->right);
        int ans=1+max(left,right);
        return ans ;
        <img width="722" alt="Screenshot 2025-05-29 at 3 26 39 PM" src="https://github.com/user-attachments/assets/8c23bb4d-c3b4-4791-b076-9d02d214c8d9" />

