筛选
==========
返回一个列表，列表中只包含原数组的"X"和"Y"，相对位置保持不变。

- for-each loop
.. code-block:: java

  public ArrayList<String> getList(String[] tokens) {
    ArrayList<String> result = new ArrayList<String>();
    for(String s: result) {
        if(s.equals("x") || s.equals("y")) {
            result.add(s);
        }
    }
    return result;
}
