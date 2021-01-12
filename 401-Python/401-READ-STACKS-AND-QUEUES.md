# READ STACKS AND QUEUES.

### What is a Stack?

- A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

- Stacks follow the FILO rule: First in last out.

### Stack Visualization

![Stack](/images/stack1.png)

### Push O(1)

- Pushing a Node onto a stack will always be an `O(1)` operation. This is because it takes the same amount of time no matter how many Nodes `(n)` you have in the stack.

### Pop O(1)

- Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

### Peek O(1)

- When conducting a peek, you will only be inspecting the top Node of the stack.

## What is a Queue

1. Enqueue - Nodes or items that are added to the queue.

2. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.

3. Front - This is the front/first Node of the queue.

4. Rear - This is the rear/last Node of the queue.

5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.

6. IsEmpty - returns true when queue is empty otherwise returns false.