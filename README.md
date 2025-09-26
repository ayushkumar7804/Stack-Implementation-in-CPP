# 🚀 Stack Implementation in C++

## 🎯 Objective
Understand and implement **Queue** and **Stack** data structures in C++ using arrays, while exploring their differences in memory management, processing order, and efficiency.

---

## 📚 Concepts

### Queue
A **Queue** is a linear data structure operating on a **FIFO (First In, First Out)** basis: elements are added at the rear and removed from the front.

- **Front**: Indicates the first element.
- **Rear**: Indicates the last element.

**Key Points:**
- FIFO ordering
- Insert at rear, remove from front
- Overflow occurs when full, underflow when empty

---

### Stack
A **Stack** is a linear data structure that operates on a **LIFO (Last In, First Out)** principle: the most recently added element is removed first.

- **Top**: Points to the latest inserted element.

**Key Points:**
- LIFO ordering
- Insert and remove only from the top
- Overflow when full, underflow when empty

---

## 📋 Queue Algorithm

1. **Start**
2. Set `front = -1`, `rear = -1`, declare array `arr[SIZE]`
3. Present menu:
   - Enqueue
   - Dequeue
   - Display
   - Peek
   - Check if Empty
   - Check if Full
   - Size
   - Clear
   - Exit
4. **Loop until Exit:**
   - Get user selection

   **Enqueue:**
   - If `rear == SIZE - 1` → Overflow
   - Else if `front == -1` → set `front = 0`
   - Increment `rear`, store element at `arr[rear]`

   **Dequeue:**
   - If `front == -1 OR front > rear` → Underflow
   - Else display `arr[front]`, increment `front`
   - If `front > rear` → reset both to -1

   **Display:**
   - If empty, show message
   - Else display elements from `front` to `rear`

   **Peek:**
   - If empty, show message
   - Else display `arr[front]`

   **Check if Empty:**
   - If `front == -1 OR front > rear` → Empty
   - Else Not Empty

   **Check if Full:**
   - If `rear == SIZE - 1` → Full
   - Else Not Full

   **Size:**
   - If empty → 0
   - Else `rear - front + 1`

   **Clear:**
   - Set both to -1

   **Exit:** 
   - End program

5. **End**

---

## 📋 Stack Algorithm

1. **Start**
2. Set `top = -1`, declare array `arr[MAX]`
3. Present menu:
   - Push
   - Pop
   - Display
   - Exit
4. **Loop until Exit:**
   - Get user selection

   **Push:**
   - If `top == MAX - 1` → Overflow
   - Else increment `top`, store element at `arr[top]`

   **Pop:**
   - If `top == -1` → Underflow
   - Else display `arr[top]`, decrement `top`

   **Display:**
   - If `top == -1` → Empty
   - Else display elements from `top` to `0`

   **Exit:** 
   - End program

   **Invalid Option:** 
   - Show error

5. **End**

---

## 🌟 Applications

### Queue
- CPU and disk scheduling
- Data buffering (I/O, print queues)
- Graph traversal (BFS)
- Order processing

### Stack
- Expression evaluation (prefix, postfix)
- Managing function calls (recursion)
- Undo/Redo features
- Backtracking algorithms
- Browser history
- Syntax parsing

---

## 🧠 Summary

- **Queue**: Follows FIFO; ideal for scheduling and buffering tasks.
- **Stack**: Follows LIFO; essential for recursion, parsing, and backtracking.
- Both are foundational data structures in computer science, each suited for different problem-solving scenarios.
