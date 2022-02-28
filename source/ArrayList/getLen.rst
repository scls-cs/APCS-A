求和
==========
计算字符串列表中所有字符串的总长度。

- for-each loop
.. code-block:: java

  public int getLen(ArrayList<String> list) {
      int total = 0;
      for(String str: list){
          total += str.length();
      }
      return total;
  }
