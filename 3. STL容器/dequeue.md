deque是双端队列，比较vector他的插入删除效率更高

构造函数

    deque<T> deqT;//默认构造形式
    deque(beg, end);//构造函数将[beg, end)区间中的元素拷贝给本身。
    deque(n, elem);//构造函数将n个elem拷贝给本身。
    deque(const deque &deq);//拷贝构造函数。

插入删除

    push_back(elem);//在容器尾部添加一个数据
    push_front(elem);//在容器头部插入一个数据
    pop_back();//删除容器最后一个数据
    pop_front();//删除容器第一个数据
    insert(pos,elem);//在pos位置插入一个elem元素的拷贝，返回新数据的位置。
    insert(pos,n,elem);//在pos位置插入n个elem数据，无返回值。
    insert(pos,beg,end);//在pos位置插入[beg,end)区间的数据，无返回值。
 

 其他方法类似vector
 
    front
    back
    empty
    clear
    erase
