#include <stdio.h>
#include <stdlib.h>

#define MAX 5  // Maximum capacity of the stack

int stack[MAX];
int top = -1;

// Function prototypes
int isFull() { return top == MAX - 1; }
int isEmpty() { return top == -1; }

void push(int value) {
    if (isFull()) printf("Stack Overflow!\n");
    else stack[++top] = value;
}
int pop() {
    if (isEmpty()) { printf("Stack Underflow!\n"); return -1; }
    else return stack[top--];
}

void display() {
    if (isEmpty()) printf("Stack is empty.\n");
    else {
        for (int i = top; i >= 0; i--) printf("%d ", stack[i]);
        printf("\n");
    }
}

int main() {
    // Basic driver to test push(10), push(20), pop(), display()
    push(10); push(20);
    printf("Popped: %d\n", pop());
    display();
    return 0;
    }
