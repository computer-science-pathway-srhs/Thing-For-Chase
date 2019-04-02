# Thing-For-Chase
I hate you chase you dummy
if (root == null) { 
            root = new Node(key); 
            return root; 
        } 
  
        /* Otherwise, recur down the tree */
        if (key.compareTo(root.key) < 0) 
        {
            root.left = insertRec(root.left, key); 
        }
        else if (key.compareTo(root.key) >= 0) 
        {
            root.right = insertRec(root.right, key); 
        }
  
        /* return the (unchanged) node pointer */
        return root; 
