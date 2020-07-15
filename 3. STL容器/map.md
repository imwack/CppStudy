map是一种映射关系，和其他语言中的字典是一样的，即Key到Value的映射
实现机制和set一样也是RB-Tree，树的节点为一个pair，pair.first为key，pair.second为value

multimap是可以有重复key的map

map<T1, T2> m;//map默认构造函数: 
map(const map &mp);//拷贝构造函数

插入数据的方法

    map.insert(pair<T1,T2>()); //往容器插入元素 
    map<int, string> mapStu;
    // 第一种 通过pair的方式插入对象
    mapStu.insert(pair<int, string>(1, "1"));
    // 第二种 通过pair的方式插入对象
    mapStu.inset(make_pair(2, "2"));
    // 第三种 重载了[]运算符
    mapStu[3] = "3";
 
查找

    find(key);//查找键key是否存在,若存在，返回该键的元素的迭代器；/若不存在，返回map.end();
    count(keyElem);//返回容器中key为keyElem的对组个数。
    lower_bound(keyElem);//返回第一个key>=keyElem元素的迭代器。
    upper_bound(keyElem);//返回第一个key>keyElem元素的迭代器。
    equal_range(keyElem);//返回容器中key与keyElem相等的上下限的两个迭代器。 

    clear();//删除所有元素
    erase(pos);//删除pos迭代器所指的元素，返回下一个元素的迭代器。
    erase(keyElem);//删除容器中key为keyElem的对组。 