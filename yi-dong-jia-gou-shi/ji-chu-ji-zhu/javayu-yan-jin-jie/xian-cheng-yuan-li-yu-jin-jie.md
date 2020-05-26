# 线程原理与进阶
## 基础概念
CPU核心数、时间碎片机制、并发与并行
 ### 认识java里的线程
  #### Java默认是多线程
  #### 实现线程启动方式 
  * 继承Thread
  * Runnable不是线程，是任务，不能运行，需要寄托Thread
  * 实现 Callable接口，是任务，需要寄托Thread
  
>只有.start()方法，才能证明是线程

  #### 线程停止【和谐的停止线程】
   * run函数运行结束时候end Thread【最和谐的方式】
   * interrupt()、isInterrupted()、static变量控制isRunning
   * Runnable直接使用Thread.currentThread().isInterrupted()
   
  #### 线程控制顺序
  

