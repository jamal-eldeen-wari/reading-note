# Stacks In Java:
Is a linear data structure that consists of Nodes where each node is a references to the next Node in the stack, but does not reference its previous.

Below are Some common terminology:
1. Push: Nodes or items that are put into the stack are pushed.
2. Pop - Nodes or items that are removed from the stack are popped. 
3. Top - This is the top of the stack.
4. Peek - When you peek you will view the value of the top Node in the stack. 
5. IsEmpty - returns true when stack is empty otherwise returns false.

Stacks has two important concepts:
1. **FILO: First In Last Out**: This means that the first item added in the stack will be the last item popped out of the stack.
2. **LIFO: Last In First Out**: This means that the last item added to the stack will be the first item popped out of the stack.

Explaining Some Stack terminology:

Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.
When we want to add a node to the stack we use push it into the stack by assigning it as the new top, with its next property equal to the original top.

Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user. But before we start with pop we need to check if the stack is empty or not.O(1)

Peeking: When conducting a peek, you will only be inspecting the top Node of the stack. Same thing as we did in the popping we check if the stack is empty or not.

# Queues in Java:
It is a linear data structure similar to the linked list and stack here are some Common terminology for a queue is:
1. Enqueue - Nodes or items that are added to the queue.
2. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty - returns true when queue is empty otherwise returns false.

Two Important concepts for queue:
1. **FIFO: First In First Out**: This means that the first item in the queue will be the first item out of the queue.
2. **LILO: Last In Last Out**: This means that the last item in the queue will be the last item out of the queue.

Explaining some terminology for Queue:

Enqueue O(1): It is similar to the stack when it comes to push elements to the stack. it adds an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n).

Dequeue O(1): When you remove an item from a queue. This is done with an O(1) operation in time because it doesn’t matter how many other items are in the queue, you are always just removing the front Node of the queue. We need to check if the queue is empty or not.

Peek O(1): When conducting a peek, you will only be inspecting the front Node of the queue. We need to check if the queue is empty or not.
