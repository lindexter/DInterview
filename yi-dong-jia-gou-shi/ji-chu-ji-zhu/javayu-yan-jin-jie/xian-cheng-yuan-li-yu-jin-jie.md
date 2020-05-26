# 线程原理与进阶

## 基础概念

CPU核心数、时间碎片机制、并发与并行

### 认识java里的线程

#### Java默认是多线程

#### 实现线程启动方式

* 继承Thread
* Runnable不是线程，是任务，不能运行，需要寄托Thread
* 实现 Callable接口，是任务，需要寄托Thread

> 只有.start\(\)方法，才能证明是线程

#### 线程停止【和谐的停止线程】

* run函数运行结束时候end Thread【最和谐的方式】
* interrupt\(\)、isInterrupted\(\)、static变量控制isRunning
* Runnable直接使用Thread.currentThread\(\).isInterrupted\(\)

#### 线程控制顺序

join来控制，让线程获取执行力，使线程做到顺序执行

> 在Java中不能指定CPU去执行某个线程，C语言调用系统的内核API才能指定

#### 线程生命周期

![](/assets/移动架构师-基础技术-Java进阶-线程原理-1.png)

#### 线程守护进阶

子线程开启守护线程,会根据main线程的结束而跟着结束

#### 线程sleep和wait区别
sleep无条件休眠,wait是等待条件
sleep休眠时间一过,重新取得执行权资格,不一定马上执行,取决于系统的资源调度
wait是等待条件符合的唤醒,唤醒后才会有执行权资格



