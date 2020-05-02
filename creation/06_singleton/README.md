# 单例模式

大名鼎鼎的单例模式，永远返回相同内存位置的绝对的、同一个实例对象。

Go有两种常见的单例模式：

+ 使用懒惰模式的单例模式，使用`once.Do()`的双重同步检查保证线程安全生成单实例

+ 使用初始化的`init(){}`能力保证只生成一个实例