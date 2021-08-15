# Reading 15: Tree


                Tree is also a node-based data structure 
                Tree can have any number of children (next values) k
                a linked list is a special case of Tree, K=1 
                In Binary tree K=2
                In the linked list head was the root but here it's Root and its node.
                Tree keeps track of the root. 
                Edges => one node to another, usually drawn as lines max 2 for binary trees 
                Leaf => Node with no edges
                Name of our edges are left and right (child)
                Height amount of edges from root to the furthest leaf(2 when 2 edges)
                3^k =nodes 
                3^2=6 nodes => k=2 is the height
                3^1=3 nodes => K=1 is the height 


                Depth First: instead of checking all nodes go to next level then right/left
                Pre order : root >> left>> right  (each one with an operation)
                left is subtree first node would be root (new root of a new tree) and a gain go to left (until there is no left)
                then go right of subtree:  root >> left>> right
                think simlarly for in order: left >> root>> right
                                Post-order: left>>right>>root 


                Depth-first => Using stack continue where you left, a lot more to check and see it visually here : https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html











