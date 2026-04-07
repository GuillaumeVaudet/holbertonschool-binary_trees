# holbertonschool-binary_trees

## Display function

The file `binary_tree_print.c` is provided to visualization purposes during development only. It is not used during the correction.

### Prototype

```c
void binary_tree_print(const binary_tree_t *tree);
```

### Usage
1. Include it in the compilation alongside your task file.
```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 binary_tree_print.c 0-binary_tree_node.c main.c -o test
```
2. Call the function in the main.c to visualize the tree
```c
#include "binary_trees.h"

int main(void)
{
    binary_tree_t *root;

    root = binary_tree_node(NULL, 6);
    root->left = binary_tree_node(root, 1);
    root->right = binary_tree_node(root, 8);

    binary_tree_print(root);
    return (0);
}
```

### Example

```
                           .----------------------(006)------.
                      .--(001)-------.                  .--(008)--.
                 .--(-02)       .--(003)-------.       (007)    (009)
       .-------(-06)          (002)       .--(005)
  .--(-08)--.
(-09)     (-07)
```

## Authors

- Leo Lebtahi
- Guillaume Vaudet