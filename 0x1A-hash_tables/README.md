# The ALX project solutions to: 0x1A. C - Hash tables
--------

> <b>For this project, my key learnings are implementing the hash functions and hash tables in `C`.</b>


> <b>The prototypes of all functions used in the project are contained in the  header file called</b> [hash_tables.h](./hash_tables.h)


> <b>Similarly, the following data structures are used in the project:</b>
                
                
                /**
                 * struct hash_node_s - Node of a hash table
                 *
                 * @key: The key, string
                 * The key is unique in the HashTable
                 * @value: The value corresponding to a key
                 * @next: A pointer to the next node of the List
                 */
                typedef struct hash_node_s
                {  
                     char *key;
                     char *value;
                     struct hash_node_s *next;
                } hash_node_t;
                
                /**
                 * struct hash_table_s - Hash table data structure
                 *
                 * @size: The size of the array
                 * @array: An array of size @size
                 * Each cell of this array is a pointer to the first node of a linked list,
                 * because we want our HashTable to use a Chaining collision handling
                 */
                typedef struct hash_table_s
                {
                     unsigned long int size;
                     hash_node_t **array;
                } hash_table_t;


> <b>All feedbacks, comments and suggestions are highly welcome. Please take a look at my codes.</b>
