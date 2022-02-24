反转
==========

将数组反转过来并且返回新数组

- 创建新数组(for-loop)
.. code-block:: java

  public int[] reverseFor(int[] array) {
    int length = array.length;
    int[] result = new int[length];
    for(int i=0; i<length; i++) {
      result[i] = array[length-1-i];
    }
    return result;
  }


- 创建新数组(while-loop)
.. code-block:: java

  public int[] reverseWhile(int[] array) {
    int length = array.length;
    int[] result = new int[length];
    int i = 0;
    while(i<length) {
      result[i] = array[length-1-i];
      i++;
    }
    return result;
  }

- 不创建新数组

.. code-block:: java

  public int[] reverse(int[] array) {
    int i = 0, j=array.length-1;
    while(i<j) {
      int temp = array[i];
      array[i] = array[j];
      array[j] = temp;
      i++;
      j--;
    }
    return array;
  }