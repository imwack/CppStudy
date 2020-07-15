set顾名思义是一个集合
数学上的定义 形如{a,b,c} 其中没有重复项目，底层实现是RB Tree,查找效率高（log n)的树形结构

mulitset是允许有多个重复项的set，例如{a,a,b,c}

    set<T> st;//set默认构造函数：
    mulitset<T> mst; //multiset默认构造函数: 
    set(const set &st);//拷贝构造函数

常用操作

    insert(elem);//在容器中插入元素。
    clear();//清除所有元素
    erase(pos);//删除pos迭代器所指的元素，返回下一个元素的迭代器。
    find(key);//查找键key是否存在,若存在，返回该键的元素的迭代器；若不存在，返回set.end();
    count(key);//查找键key的元素个数
    lower_bound(keyElem);//返回第一个key>=keyElem元素的迭代器。
    upper_bound(keyElem);//返回第一个key>keyElem元素的迭代器。
    equal_range(keyElem);//返回容器中key与keyElem相等的上下限的两个迭代器。
 