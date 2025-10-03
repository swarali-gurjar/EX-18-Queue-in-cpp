# Aim: To study and implement Queue implementation using array

## Theory:

A queue is a linear data structure where new elements are always added at one end, called the rear, and removed from the other end, called the front.

It works on the FIFO (First In, First Out) principle — meaning the first item that goes into the queue is also the first one to come out, much like people standing in a line.

Adding an element to the queue is known as enqueue, while removing an element is called dequeue.

A circular queue is a more efficient form of the regular queue, where the front and rear are linked together. This helps reuse empty spaces created when elements are removed, solving the problem of wasted memory in a simple linear queue.

## Algorithm:

**Step 1**: Initialization-

- Define a constant SIZE as the maximum capacity of the queue.

Create a class Queue with:

- An integer array arr[SIZE] to store queue elements.

- Two integer variables front and rear initialized to -1.

**Step 2**: Enqueue Operation (Insert Element)-

Check for Overflow:

- If rear == SIZE - 1, print "Queue Overflow!" and exit.

Insert First Element:

- If front == -1, set front = 0.

Insert Element:

- Increment rear and assign arr[rear] = value.

- Print that the value has been inserted.

**Step 3**: Dequeue Operation (Remove Element)-

Check for Underflow:

- If front == -1 or front > rear, print "Queue Underflow!" and exit.

Remove Element:

- Print the element at arr[front] as removed.

- Increment front.

**Step 4**: Display Queue Elements-

Check if Queue is Empty:

- If front == -1 or front > rear, print "Queue is empty." and exit.

Print Elements:

- Loop from front to rear and print each element in arr.

**Step 5**: Main Function Execution-

Create a Queue object q.

Perform the following operations:

- enqueue(10)

- enqueue(20)

- enqueue(30)

- display()

- dequeue()

- display()

- enqueue(40)

- display()

**Step 6**: End

## Conclusion

By implementing a queue using arrays, we understood how the FIFO (First In, First Out) principle works in data structures.
The program demonstrated the basic operations of a queue, namely enqueue (insertion) and dequeue (deletion), along with checking conditions like overflow and underflow. 
This experiment helped us learn how queues can be efficiently managed using arrays and laid the foundation for more advanced variations like the circular queue.
