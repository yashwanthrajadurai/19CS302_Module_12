# EX 58 C Function to display queue elements using Linked List.(use integer data in the queue)

## AIM:

To write a C Function to display queue elements using Linked List.

## Algorithm

Start.

Define a variables.

Write a program to display queue elements using linked list.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End

## Program:

struct Node

{

int data;

struct Node *next;

}*front=NULL,*rear=NULL; 

void display()

{

struct Node *temp=front; 

if(temp==NULL)

{

printf("queue is empty\n");

}

else
{

while(temp!=NULL)

{

printf("%d\n",temp->data); 

temp=temp->next;

}

}



## Output:

![image](https://github.com/user-attachments/assets/91d73349-5532-4090-b44a-835351fd2b39)


## Result:

Thus the program was executed and the output was verified successfully.
