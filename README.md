# Threads and Multithreading Laboratory

**Implementing Threads and Multithreading Using Python and GitHub**

## Student Information

- **Name:** JC Ree F. Redelosa
- **Section:** B186
- **Date:** November 7, 2026
- **Programming Language:** Python 3.x
- **Development Environment:** Visual Studio Code
- **Repository:** Threads-and-Multithreading-Lab

---

## I. Laboratory Overview

This laboratory activity demonstrates the implementation of threads and multithreading using Python's built-in `threading` module. It explores how multiple threads can execute concurrently, how thread synchronization works using `join()`, and how shared resources can be protected using `threading.Lock()`.

The project also uses GitHub for source code management, file organization, and submission of the completed laboratory activities.

## II. Learning Objectives

After completing this laboratory, the student should be able to:

- Explain the concepts of threads and multithreading.
- Create and execute threads using Python.
- Implement multiple threads for concurrent execution.
- Demonstrate thread synchronization using `join()`.
- Manage shared resources using thread locks.
- Understand and prevent race conditions.
- Upload and manage programming projects using GitHub.

## III. Project Structure

```text
Threads-and-Multithreading-Lab/
│
├── README.md
├── LAB_GUIDE.md
│
├── task1_single_thread.py
├── task2_multiple_threads.py
├── task3_thread_synchronization.py
├── task4_thread_lock.py
│
└── screenshots/
    ├── task1_screenshot.png
    ├── task2_screenshot.png
    ├── task3_screenshot.png
    └── task4_screenshot.png
```

## IV. Laboratory Activities

### Task 1: Creating and Executing a Single Thread

This activity demonstrates how to create and execute a single thread using `threading.Thread()`.

The program displays numbers from 1 to 5, with a one-second delay between each number. The `start()` method executes the thread, while `join()` ensures that the main program waits until the thread finishes.

**Expected Output:**
```text
Number: 1
Number: 2
Number: 3
Number: 4
Number: 5
Program completed.
```

**Screenshot:**

![Task 1 Screenshot](screenshots/task1_screenshot.png)

### Task 2: Implementing Multiple Threads

This activity demonstrates concurrent execution using two separate threads. Each thread executes its own function and displays numbers from 1 to 5.

The output order may vary because the operating system scheduler determines when each thread executes.

**Expected Output:**
```text
Thread 1: 1
Thread 2: 1
Thread 1: 2
Thread 2: 2
...
Both threads completed.
```

**Screenshot:**

![Task 2 Screenshot](screenshots/task2_screenshot.png)

### Task 3: Thread Synchronization Using join()

This activity demonstrates how the `join()` method synchronizes thread execution.

A worker thread simulates downloading a file using `time.sleep(3)`. The main program waits for the download thread to finish before continuing.

**Expected Output:**
```text
Downloading file...
Main program is waiting...
Download completed.
Main program continues.
```

**Screenshot:**

![Task 3 Screenshot](screenshots/task3_screenshot.png)

### Task 4: Managing Shared Resources Using Thread Locks

This activity demonstrates how multiple threads access and modify a shared variable.

Two threads increment a shared counter 100,000 times each. The `threading.Lock()` mechanism protects the critical section and prevents conflicting updates.

**Expected Output:**
```text
Final Counter: 200000
```

**Screenshot:**

![Task 4 Screenshot](screenshots/task4_screenshot.png)

## V. Technologies Used

- **Python 3.x** – Programming language used to implement the laboratory activities.
- **Threading Module** – Used to create, manage, and synchronize threads.
- **Visual Studio Code** – Development environment for writing and executing Python programs.
- **GitHub** – Used for source code storage, version control, and project submission.

## VI. How to Run the Programs

1. Install Python 3.x.
2. Download or clone this repository.
3. Open the project folder in Visual Studio Code.
4. Open the integrated terminal.
5. Execute each Python program using the following commands:

**Task 1:**
```bash
python task1_single_thread.py
```

**Task 2:**
```bash
python task2_multiple_threads.py
```

**Task 3:**
```bash
python task3_thread_synchronization.py
```

**Task 4:**
```bash
python task4_thread_lock.py
```

## VII. Key Concepts Demonstrated

| Concept | Description |
|---|---|
| Thread | An independent execution unit within a process. |
| Multithreading | Running multiple threads within one process. |
| start() | Starts the execution of a thread. |
| join() | Makes the calling thread wait for another thread to finish. |
| Lock() | Prevents multiple threads from entering a protected section simultaneously. |
| Shared Resource | Data or objects accessed by multiple threads. |
| Race Condition | An error that may occur when concurrent operations interfere with each other. |
| Critical Section | A section of code that accesses shared resources and requires protection. |

## VIII. Learning Outcomes

Through this laboratory activity, I successfully implemented single-thread and multiple-thread execution using Python. I also demonstrated thread synchronization using the `join()` method and protected shared data using `threading.Lock()`.

The activities helped me understand how threads execute concurrently, how synchronization coordinates their execution, and why locks are important in preventing race conditions and maintaining data consistency.

## IX. Conclusion

This laboratory activity provided practical experience in implementing threads and multithreading using Python. Through the four activities, I learned how to create threads, execute multiple tasks concurrently, synchronize thread execution, and manage shared resources safely.

Overall, the laboratory strengthened my understanding of concurrent programming and demonstrated the importance of proper thread management in developing reliable and responsive applications.

---

**Laboratory Activity: Implementing Threads and Multithreading Using Python and GitHub**

**Status:** Completed
