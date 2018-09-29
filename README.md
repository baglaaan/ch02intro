# ch02intro
Introduction to OS, Chapter 02

Read [Introduction to OS](http://pages.cs.wisc.edu/~remzi/OSTEP/intro.pdf) and answer the following review questions.

1. **What is an operating system? What does it do?**  There is a body of software, in fact, that is responsible for making it
easy to run programs (even allowing you to seemingly run many at the same time
same time), allowing programs to share memory, enabling programs to
interact with devices. That body of software is called the operating system.
In fact, there are many programs that are responsible for its creation
easy-to-launch programs (even allowing you to seemingly run a lot
at the same time), allowing programs to exchange memory, allowing programs
interact with devices and other fun things. This software module is called the operating system.
2. **What is virtualization?** The main way of operating the OS is a common method that
we call virtualization.
3. **How does an OS provide access to its features?** This is hardware management, program management, data access, management of system resources, network communication. Hardware management: one of the most important functions of the operating system is the management of all internal and external equipment of the computer. The operating system monitors all connected devices, tells them how to work and interact. Program management: Operating systems also run programs, allowing them to work and function in accordance with the developed ones. Access to data. The operating system is also responsible for accessing, storing and retrieving data on the hard disk of the computer. Management of system resources. Key operations are given priority based on presets within the operating system that determine the importance of the process or program. Network communication. The operating system also facilitates network communication, allowing connected network devices to communicate with the computer and any programs that require them. The OS provides hundreds of system calls available to applications, these calls run programs, access memory, devices
4. **What illusion does a virtualized CPU provide?** The operating system, with some help from hardware,
responsible for this illusion, that is, the illusion that the system has
a very large number of virtual processors. Rotate one processor (or a small set
them) into a seemingly endless number of processors and, thus, allowing many
programs that seem to run immediately - this is what we call processor virtualization


    - **How does this affect the user experience?** Of course, to run programs and stop them, and otherwise talk about which programs should be run, there must be some interfaces (APIs) that you can use to transfer your OS desires.
    - **How does this affect the developer experience?** You may also notice that the ability to run multiple programs simultaneously raises new questions. For example, if two programs want to work at a certain time, which should be performed? The OS policy answers this question; policies are used in many different places in the OS to answer these types of questions, and therefore we will study them when we learn about the basic mechanisms that implement operating systems (for example, the possibility of running several programs at once). Hence the role of the OS as a resource manager.
    - **What if the CPU were not virtualized?** The operating system will not be able to more effectively and efficiently use the processor's power in the computer to make it work slowly. This is also a requirement for many programs for virtual machines and should be included so that they do not work properly or even at all.
5. **What is a memory address?** A memory address is a reference to a specific memory location used at different levels by software and hardware.
6. **What is memory virtualization?** The OS takes a physical resource (for example, a processor, memory or disk) and converts it into a more general, powerful and easy-to-use virtual form.
    - **Why would we want this?** Physical memory is “limited”, so then aggregates those resources into a virtualized memory pool available to any computer in the cluster. 


8. **What happens if you write a C/C++ program that writes past the end of an array?**  your answer goes here
     
9. **What is a thread?** 
The execution thread is the smallest processing unit whose execution can be assigned by the operating system kernel. The implementation of threads of execution and processes in different operating systems differs from each other, but in most cases the execution thread is inside the process.

10. **Why would we ever write a multi-threaded program?** The problems of concurrency are no longer limited to the OS itself. Indeed, modern multi-threaded programs demonstrate the same problems. The main program creates two threads using Pthread create () 6. You can think of a thread as a function that works in the same memory space as other functions, more than one of which is active at the same time.
11. **What is atomicity?** Atomicity is a feature of databases systems dictating where a transaction must be all-or-nothing.

    - **Is a C/C++ statement atomic?** C/C++ has atomic operations. Atomic types are those for which reading and writing are guaranteed to happen in a single instruction. 

    - **Is a Java statement atomic?** The classes in the package java.util.concurrent use atomic methods to update their internal state in a thread-safe way.  
    - **Is an assembler statement atomic?**  Atomic Assembler is a machine that allows you to legitimately duplicate any item by assembling it using Strange Matter substances. The duplication takes a long time and requires a lot of energy to do so.


13. **What does persistence mean?** DRAM stores data in a volatile manner, hard drives and solid-state drives are good for storing long-lived information ,file system within OS manages disks


14. **How does OS hard drive virtualization differ from CPU & memory virtualization?** Virtual hard disk file contains a file system and can contain an operating system, applications, and data. Virtual hard disk files are usually attached to virtual machines (virtual machines) and function as system or disk drives for computer science VM & In, memory virtualization separates volatile memory resources (RAM) from individual systems in the data center, and then aggregates these resources into a virtual memory pool, accessible to any computer in the cluster.
15. **How does running multiple programs at the same time increase CPU efficiency?**You can also notice that the ability to run multiple programs at once
raises all new questions. For example, if two programs run at a specific time, which should be performed? This question is answered OS policy; policies are used in many places within OS to answer these types of questions, and therefore we will study them as we learn about the basic mechanisms that implement operating systems (for example, the ability to run several programs at once). Hence the role of OS as a resource manager.
16. **What is multiprogramming?** Multiprogramming is a rudimentary form of parallel processing, in which several programs are simultaneously launched on a uniprocessor computer. In particular, multiprogramming has become commonplace because of the desire to better use machine resources.
