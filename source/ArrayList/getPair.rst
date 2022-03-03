一对元素
==========
返回一个列表，列表中的元素为数组的元素对，要求保持相对位置不变。

例子：

参数：{"a", "b", "c"} （数组类型）

返回：{"a+b", "a+c", "b+c"} (动态数组类型)


.. code-block:: java

  public ArrayList<String> getPair(String[] array) {
      ArrayList<String> result = new ArrayList<String>();
      for(int i=0; i<array.length-1; i++) {
          for(int j=i+1; j<array.length; j++) {
            String x = array[i] + "+" + array[j];
            result.add(x);
          }
      }
      return result;
  }