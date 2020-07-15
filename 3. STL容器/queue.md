queue是一种先进先出的数据结构，底层实现也是dequeue

构造函数

    queue<T> q;//queue采用模板类实现，queue对象的默认构造形式：
    queue(const queue &que);//拷贝构造函数

操作

    push(elem);//往队尾添加元素
    pop();//从队头移除第一个元素
    back();//返回最后一个元素
    front();//返回第一个元素