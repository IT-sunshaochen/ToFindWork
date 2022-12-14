<!--
 * @Author: sunshaochen 805960031@qq.com
 * @Date: 2022-11-01 09:38:10
 * @LastEditors: sunshaochen 805960031@qq.com
 * @LastEditTime: 2022-11-01 14:25:45
 * @FilePath: \ToFindWork\OS基础.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
从用户的角度来看，进程是正在运行的程序实例，而线程是进程中真正执行任务的基本单位。也就是说一个运行的程序至少包含一个进程，一个进程至少包含一个线程，线程不能独立于进程而存在。
进程编号 PID：进程的身份标识。
进程的状态：
新建状态
就绪状态
运行状态
阻塞状态
销毁状态
进程和线程的区别
进程和线程的区别主要体现在以下几点。

区别1：从属关系不同
从属关系不同：进程是正在运行程序的实例，进程中包含了线程，而线程中不能包含进程。

区别2：描述侧重点不同
描述侧重点不同：进程是操作系统分配资源的基本单位，而线程是操作系统调度的基本单位。

区别3：共享资源不同
共享资源不同：多个进程间不能共享资源，每个进程有自己的堆、栈、虚存空间（页表）、文件描述符等信息，而线程可以共享进程资源文件（堆和方法区）。

区别4：上下文切换速度不同
上下文切换速度不同：线程上下文切换速度很快（上下文切换指的是从一个线程切换到另一个线程），而进程的上下文切换的速度比较慢。

区别5：操纵者不同
操纵者不同：一般情况下进程的操纵者是操作系统，而线程的操纵者是编程人员。


死锁的产生需要满足以下 4 个条件：

互斥条件：指运算单元（进程、线程或协程）对所分配到的资源具有排它性，也就是说在一段时间内某个锁资源只能被一个运算单元所占用。
请求和保持条件：指运算单元已经保持至少一个资源，但又提出了新的资源请求，而该资源已被其它运算单元占有，此时请求运算单元阻塞，但又对自己已获得的其它资源保持不放。
不可剥夺条件：指运算单元已获得的资源，在未使用完之前，不能被剥夺。
环路等待条件：指在发生死锁时，必然存在运算单元和资源的环形链，即运算单元正在等待另一个运算单元占用的资源，而对方又在等待自己占用的资源，从而造成环路等待的情况。
只有以上 4 个条件同时满足，才会造成死锁。


进程之间的通信方式有：无名管道( pipe )、高级管道（popen）、有名管道（named pipe）、消息队列( message queue )、信号量( semophore ) 、信号 ( sinal ) 、共享内存( shared memory ) 、套接字( socket )。
线程通信是管道和消息队列MQ