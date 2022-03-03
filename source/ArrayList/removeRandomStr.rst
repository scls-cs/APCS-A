删除随机元素
==========
随机删除列表中的一个元素并返回该元素。

例子：

列表：["a", "d", "b", "c", "e"] （动态数组类型）

返回："b"

列表变为["a", "d" , "c", "e"]


.. code-block:: java

public String removeRandomStr(ArrayList<String> list) {
  if(list.size()>0) {
    return list.remove((int)(Math.random()*list.size()));
  }
  return "None";
}