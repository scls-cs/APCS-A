括号平衡
==========
判断列表中的括号是否平衡。

平衡需要满足两个条件：

1. 在任意位置上，已出现的右括号的数量不能超过左括号数量。

2. 列表中左括号数量与右括号数量相等。

例如：["(",  ")",  ")",  "("]不是一个平衡括号，违反了条件1。

["(",  ")",  "(",  "("]也不是一个平衡括号，违反了条件2。

["(",  ")",  "(",  ")"], ["(",  "(",  ")",  ")"]均为平衡括号。


输入：

列表：["a", "a", "b", "c", "a"] （动态数组类型）

输出：true or false



.. code-block:: java

  public boolean isBalanced(ArrayList<String> tokens) {
    int openCount = 0;
    int closeCount = 0;
    for(String str: tokens) {
      if(str.equals("(")) {
          openCount++;
      } else {
          closeCount++;
      }
      if(closeCount > openCount) {
          return false;
      }
    }
    return openCount == closeCount;
  }