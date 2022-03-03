改变或者删除动态数组元素
==========
如果字符串是回文字符串，则删除该元素；否则则用反转后的字符串替换该元素。

输入：["ABBA",  "CD",  "dd"](动态数组类型）

列表变为["CD"]

字符串反转算法见：:ref:`reverse_string`.

- for loop
.. code-block:: java

  public void changeOrRemoveFor(ArrayList<String> list) {
    for(int i=list.size()-1; i>=0; i--) {
      String cur = list.get(i);
      if(reverse(cur).equals(cur)) {
          list.remove(i);
      } else {
          list.set(i, reverse(cur));
      }
    }
  }

- while loop
.. code-block:: java

  public void changeOrRemove(ArrayList<String> list) {
    int i = list.size()-1;
    while(i>=0) {
      String cur = list.get(i);
      if(reverse(cur).equals(cur)) {
          list.remove(i);
      } else {
          list.set(i, reverse(cur));
      }
      i--;
    }
  }
