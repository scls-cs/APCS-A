全部遍历
==========
顺序遍历二维数组中的每一个元素。

- row-major order
.. code-block:: java

  for(int row=0; row<array.length; row++) {
    for(int col=0; col<array[0].length; col++) {
      System.out.println(array[row][col]);
    }
  }

- column-major order
.. code-block:: java

  for(int col=0; col<array[0].length; col++) {
    for(int row=0; row<array.length; row++) {
      System.out.println(array[row][col]);
    }
  }

