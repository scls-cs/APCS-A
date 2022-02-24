计数
==========
统计字符串数组中与target内容相同的字符串个数。

- for-each loop
.. code-block:: java

  public int countStrings(String[] list, String target) {
    int result = 0;
    for(String str: list) {
        if(str.equals(target)) {
            result++;
        }
    }
    return result;
  }

- for loop
.. code-block:: java

  public int countStrings(String[] list, String target) {
    int result = 0;
    for(int i=0; i<list.length; i++) {
        if(list[i].equals(target)) {
            result++;
        }
    }
    return result;
  }

