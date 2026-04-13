# C++ Threading 

Threading concept discussed here are relavent to C++ language. It is different from OS.
# TOPIC: Introduction to thread in c++ (c++11)

- QUESTIONS
    1. What do you understand by thread and give one example in C++?
- ANSWER

    0. In every application there is a default thread which is main(), in side this we create other threads.
    1. A thread is also known as lightweight process. Idea is to achieve parallelism by dividing a process into multiple threads. 
    For example:
    (a) The browser has multiple tabs that can be different threads. 
    (b) MS Word must be using multiple threads, one thread to format the text, another thread to process inputs (spell checker)
    (c) Visual Studio code editor would be using threading for auto completing the code. (Intellicence)

- WAYS TO CREATE THREADS IN C++11
    1. Function Pointers
    2. Lambda Functions
    3. Functors
    4. Member Functions
    5. Static Member functions 

- Example of Function Pointers using std:thread  -> Check code    
![alt text](./Figures/intro_thread.png)


# TOPIC: Different Types Of Thread Creation And Calling.

There are 5 different types of creating threads in C++11 using **callable Objects**. 

** Note : If we create mulitple threads at the same time it doesn't guarantee which one will start first. **

1. Function Pointer : this is the very basic form of creating threads.
![alt text](./Figures/fp_create_threads.png)

2. Lambda Function
![alt text](./Figures/lambda_create_threads.png)

3. Functor (Function Object)  : Class overloading the operator ()
![alt text](./Figures/functor_create_threads.png)

4. Member function (Non_static member function) : Call a class function (non-static) using the class object. 
![alt text](./Figures/NSmember_func_create_threads.png)

5. Static member function : Directly call the static memmber function.
 ![alt text](./Figures/Smember_func_create_threads.png)
