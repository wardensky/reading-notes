# 第9章　多线程和并发

这一章需要有多线程开发的基础才能看，建议先看看《Java多线程编程实战指南（核心篇）（Java多线程编程实战系列）》。

## 建议118： 不推荐覆写start方法

## 建议119：启动线程前stop方法是不可靠的

## 建议120：不使用stop方法停止线程

## 建议121：线程优先级只使用三个等级

确实如此，只需要使用

```
MIN_PRIORITY = 1;
NORM_PRIORITY = 5;
MAX_PRIORITY = 10;
```

虽然Java定义了那么多优先级，在操作系统层面是不能保证的，用这三个就好了。

## 建议122：使用线程异常处理器提升系统可靠性

## 建议123：volatile不能保证数据同步

## 建议124：异步运算考虑使用Callable接口

## 建议125：优先选择线程池

## 建议126：适时选择不同的线程池来实现

## 建议127：Lock与synchronized是不一样的

synchronized用的是内部锁，Lock是显示锁。

## 建议128：预防线程死锁

## 建议129：适当设置阻塞队列长度

## 建议130：使用CountDownLatch协调子线程

## 建议131：CylicBarrier让多线程齐步走
