# Singly Linked List in C++

### Introduction

A **linked list** is a linear data structure where elements (**nodes**) are stored in **non-contiguous memory locations**.
Each node contains:

* **Data field:** stores the actual value.
* **Pointer field (next):** points to the next node in the list.

In a **singly linked list**, each node points only to its immediate successor, and the last node points to `NULL`.

---

## Characteristics

* Nodes are created **dynamically** using pointers.
* Traversal is **sequential** until a `NULL` pointer is reached.
* Insertions and deletions are simpler than arrays, as no shifting of elements is needed.

---

## Advantages

* **Dynamic size:** Can grow or shrink at runtime.
* **Efficient operations:** Insertions and deletions, especially in the middle, are faster.
* **Versatility:** Forms the basis for stacks, queues, and more advanced data structures.

## Disadvantages

* **Extra memory:** Pointers require additional storage.
* **Sequential access only:** No direct indexing like arrays.
* **Reverse traversal:** Not straightforward in singly linked lists.

---

## Array vs Linked List

| Feature            | Array             | Linked List                  |
| ------------------ | ----------------- | ---------------------------- |
| Memory Allocation  | Static (fixed)    | Dynamic (runtime)            |
| Insertion/Deletion | Costly (shifting) | Easy (adjusting pointers)    |
| Access Time        | O(1)              | O(n) sequential              |
| Memory Usage       | May waste space   | Exact usage                  |
| Structure          | Contiguous blocks | Non-contiguous dynamic nodes |

---

## Real-Life Applications

* Dynamic memory management
* Implementing **stacks, queues, and hash tables**
* File systems, social network connections, OS scheduling

---

## Algorithms & Program Summaries

### 1️⃣ Node Creation

**Algorithm:**

1. Define a `Node` class with `data` and `next`.
2. Dynamically create a new node.
3. Display its `data` and `next` pointer.

### 2️⃣ Linked List Traversal

**Algorithm:**

1. Dynamically create three nodes (`n1, n2, n3`).
2. Link nodes: `n1->next = n2`, `n2->next = n3`.
3. Initialize `temp = n1`.
4. While `temp != NULL`:

   * Print `temp->data`.
   * Move `temp = temp->next`.

### 3️⃣ Insertion at Head

**Algorithm:**

1. Define `insert_head(head, data)`.
2. Create a new node with the given `data`.
3. Set `new_node->next = head`.
4. Update `head = new_node`.
5. Traverse and display the updated list.

---

## Conclusion

* Singly linked lists allow **dynamic memory allocation** and **efficient insertions/deletions**.
* Nodes can be accessed sequentially using traversal.
* Insertion at the head is **faster than array insertion**.
* Singly linked lists form a **fundamental data structure** in computer science for flexible and memory-efficient data storage.

Do you want me to do that next?
