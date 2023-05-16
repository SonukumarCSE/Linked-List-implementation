# Linked-List-implementation
Simple Linked list implementation in C++


                                            Representation of Linked Lists


A linked list is represented by a pointer to the first node of the linked list. The first node is called the head node of the list. If the linked list is empty, then the value of the head node is NULL.

Each node in a list consists of at least two parts:
data
Pointer (Or Reference) to the next node


In C/C++, we can represent a node using structure. Below is an example of a linked list node with integer data.

          struct Node
          {
              int data;
              struct Node* next; 
          };

code.

    // simple linked list implementation in c++

    # include <iostream>
    using namespace std;

    struct Node
    {
        int data;
        Node *next;
        Node(int x)
        {
            data = x;
            next = NULL;
        }
    };

    int main()
    {
        Node *head = new Node(10);
        Node *temp1 = new Node(20);
        Node *temp2 = new Node(30);
        head->next = temp1;
        temp1->next = temp2;
        return 0;
    }

