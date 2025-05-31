# EX 57 C function to perfom push,pop and peek functions in Stack using Linked List.( store float data in stack)

## AIM:

To write a C function to perfom push,pop and peek functions in Stack using Linked List.

## Algorithm

Start.

Define a variables.

Write a functions to perform push, pop,peek,display, in Queue using linked list.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End   

## Program:

struct Node   

{  

int data;  

struct Node *next;  

}*head;

void push(int data)  

{ 

    struct Node*n=(struct Node*)malloc(sizeof(struct Node));
    
    if(head==NULL)
    
    {
    
    n->data=data;
    
    n->next=NULL;
    
    head=n;
    
    }
    
    else

    
    {
    
        n->data=data;
        
        n->next=head;
        
        head=n;
    
    }
    
}  

void pop()  

{ 

    struct Node*temp;
    
    if(head==NULL)
    
    {
    
        printf("stack is empty");
        
        return;
    
    }
    
    
    temp=head;
    
    head=head->next;
    
    free(temp);

}  


void display()  

{  

    struct Node*temp;
    
    if(head==NULL)
    
    {
    
        printf("stack is empty");
        
        return;
    
    }

    
    
    temp=head;
    
    printf("stack:");
    
    while(temp!=NULL)
    
    {
    
        
        printf("%d ",temp->data);
        
        temp=temp->next;
    
    }
    
    
}  

void peek()

{

printf("\nstack top:%d\n",head->data);

    
}



## Output:

![image](https://github.com/user-attachments/assets/ea5ce7d0-90c3-48a0-921a-840f850e89a4)


## Result:

Thus the program was executed and the output was verified successfully.
