极值
==========
返回数组中的最大/最小值。

- for-each loop
.. code-block:: java

  public int findMax(int[] array) {
	    int result = array[0];
	    for(int i: array) {
	        if(i>result) {
	            result = i;
	        }
	    }
	    return result;
  }

- for loop
.. code-block:: java

  public int findMax(int[] array) {
      int result=array[0];
      for(int i=0; i<array.length; i++) {
	        if(array[i] > result) {
	            result = array[i];
	        }
	    }
      return result;
  }

.. note::

  如果需要返回极值的下标，不能使用for-each循环。

