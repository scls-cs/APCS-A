遍历列
==========
将二维数组中的某一列作为一维数组返回

.. code-block:: java

  public static int[] getColumn(int index, int[][] source) {
    int[] column = new int[source.length];
      for(int row=0; row<column.length; row++) {
        column[row] = source[row][index];
      }
    return column;
  }

