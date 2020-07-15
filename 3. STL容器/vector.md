vector类似与array，但是可以动态的扩容（array大小是固定的）

扩容方式一般是new一份 size*2的空间，把当前内存拷贝过去

constructor

    vector<int> v;
    vector<int> v(n, 0);  //默认n个0
    vector<int> v(v1.begin(),v1.end()); //区间元素拷贝构造

常用的操作

    size(); //元素个数
    empty(); //是否为空
    capacity(); //容量
    reverse(n); //设置n个空间

    at(id); //第id个元素 越界则抛出异常
    [id]; //直接访问元素
    front();
    back();

    push_back(n);//添加到末尾
    pop_back();//删除最后一个
    erase(start,end);//区间删除
    erase(pos);//删除某个
    clear();
