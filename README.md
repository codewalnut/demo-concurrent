# 并发编程Demo项目

## Semaphore信号量
Semaphore用于限制可以访问某些资源（物理或逻辑的）的线程数目，他维护了一个许可证集合，有多少资源需要限制就维护多少许可证集合，假如这里有N个资源，那就对应于N个许可证，同一时刻也只能有N个线程访问。一个线程获取许可证就调用acquire方法，用完了释放资源就调用release方法。