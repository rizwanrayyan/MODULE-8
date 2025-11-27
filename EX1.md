# Ex.No:1
# Ex.Name : Complete the preorder function in your editor below, which has  parameter: a pointer to the root of a binary tree. It must print the values in the tree's preorder traversal as a single line of space-separated values.
## Date: 25/09/2025
## Aim:
To write a C++ function to perform postorder traversal on a binary tree and print the node values as a single line of space-separated values.

## Algorithm:
```
1. Start the function.

2. If the root is NULL, return.

3. Recursively traverse the left subtree.

4. Recursively traverse the right subtree.

5. Print the root node's data.

6. End the function.
```



## Program:
```cpp
void Binary_tree::posttrav(tree* t = root)
{
    if (root == NULL) {
        cout << "Nothing to display";
    }
    else if (t != NULL) {
        posttrav(t->Left);
        posttrav(t->Right);
        cout << t->info << " ";
    }
}
```

## Output:
<img width="721" height="219" alt="image" src="https://github.com/user-attachments/assets/f316b5a3-219c-43b6-946e-2c7738e9ccea" />



## Result:
The function successfully performs postorder traversal of the given binary tree and prints the node values in the order:
Left Subtree → Right Subtree → Root
