stack即数据结构中的栈，先进后出的特点，STL中是实现是一种adapter，底层数据结构是dequeue双端队列，去掉了一端的操作。

构造

    stack<T> stkT;//stack采用模板类实现， stack对象的默认构造形式： 
    stack(const stack &stk);//拷贝构造函数

常用操作

    push(elem);//向栈顶添加元素
    pop();//从栈顶移除第一个元素
    top();//返回栈顶元素
    empty();
    size();