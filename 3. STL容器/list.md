list容器是一个双向链表,相较于vector其优点是插入删除O(1)时间内完成，缺点是不能随机访问

构造函数

    list<T> l; 
    list(beg,end); 
    list(n,elem);//构造函数将n个elem拷贝给本身。
    list(const list &lst);//拷贝构造函数。
— 

常用操作

    push_back(elem);//在容器尾部加入一个元素
    pop_back();//删除容器中最后一个元素
    push_front(elem);//在容器开头插入一个元素
    pop_front();//从容器开头移除第一个元素
    insert(pos,elem);//在pos位置插elem元素的拷贝，返回新数据的位置。
    insert(pos,n,elem);//在pos位置插入n个elem数据，无返回值。
    insert(pos,beg,end);//在pos位置插入[beg,end)区间的数据，无返回值。
    clear();//移除容器的所有数据
    erase(beg,end);//删除[beg,end)区间的数据，返回下一个数据的位置。
    erase(pos);//删除pos位置的数据，返回下一个数据的位置。
    remove(elem);//删除容器中所有与elem值匹配的元素。
    reverse();//反转链表 
    sort(); //list排序
