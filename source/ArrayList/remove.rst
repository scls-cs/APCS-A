删除元素
==========
将列表中所有的str删除掉。

例子：

列表：["a", "a", "b", "c", "a"] （动态数组类型）

str: "a"

列表变为["b", "c"]


.. code-block:: java

  public void removeStr(ArrayList<String> list, String str) {
    int i = list.size()-1;
    while(i>=0) {
      if(list.get(i).equals(str)) {
          list.remove(i);
      }
      i--;
    }
  }