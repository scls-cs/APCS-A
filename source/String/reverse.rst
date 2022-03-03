.. _reverse_string:


反转字符串
==========
将字符串反转之后返回。

.. code-block:: java

  public String reverse(String str) {
    String result = "";
    for(int i=0; i<str.length(); i++) {
      result = str.substring(i, i+1) + result;
    }
    return result;
  }

