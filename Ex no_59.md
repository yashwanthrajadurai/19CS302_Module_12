# EX 59 C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.(use character data in Queue).

## AIM:

To write a C functions to perform-enqueue, dequeue, peek, display in Queue using Linked List.

## Algorithm

Start.

Define a variables.

Write a functions to perform enqueue, dequeue,peek,display, in Queue using linked list.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End

## Program:

struct Node

{

char data;

struct Node *next;

}*front=NULL,*rear=NULL; 

void enqueue(char data)

{

struct Node *n=(struct Node*)malloc(sizeof(struct Node)); 

n->data=data;

n->next=NULL; 

if(front==NULL)

{

front=rear=n;

}

else


{

rear->next=n; 

rear=n;
}

}

Void display()

{

struct Node *temp; 

temp=front; 

if(temp==NULL)

{

printf("queue elements:\n");

}

else

{

printf("queue elements:\n"); 

while(temp!=NULL)

{

printf("%c\n",temp->data); 

temp=temp->next;

}

}

}


void dequeue()

{

struct Node *temp; 

temp=front; 

if(temp==NULL)

{

printf("queue is empty\n");

}

else

{

front=temp->next; 

free(temp);

}

}

void peek(){

printf("peek:"); 

printf("%c\n",front->data);}


## Output:


![image](https://github.com/user-attachments/assets/9756311f-732a-4030-8eb4-c3c4271b172b)




## Result:

Thus the program was executed and the output was verified successfully.
