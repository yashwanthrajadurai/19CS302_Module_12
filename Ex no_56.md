# EX 56 C function to display stack elements using Linked List.(store integer data in stack) .

## AIM:

To write a C function to display stack elements using Linked List.

## Algorithm

Start.

Define a variables.

Write a program to display stack elements using linked list.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End   

## Program:

Struct Node

{

int data;

struct Node *next;

}*head;

void display()

{

struct Node *temp= head; 

while(temp!=NULL)

{

printf("%d\n",temp->data); 

temp=temp->next;

}

}


## Output:

![Screenshot 2025-05-26 173521](https://github.com/user-attachments/assets/447c3096-b7b9-403a-8c30-a479051c712f)


## Result:

Thus the program was executed and the output was verified successfully.
