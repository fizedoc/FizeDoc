=============================================
解析PHP源码，并生成对应文档格式
=============================================


+-------------+----------+
|属性         |值        |
+=============+==========+
|命名空间     |fize\\doc |
+-------------+----------+
|类名         |Doc       |
+-------------+----------+


:方法:


+-----------------+----------------------------+
|方法名           |说明                        |
+=================+============================+
|`__construct()`_ |常规调用请先初始化          |
+-----------------+----------------------------+
|`file()`_        |解析代码文件                |
+-----------------+----------------------------+
|`dir()`_         |解析代码文件夹              |
+-----------------+----------------------------+


方法
======
__construct()
-------------
常规调用请先初始化

.. code-block:: php

  public function __construct (
      string $handler
  )


:参数:
  +--------+----------------------------+
  |名称    |说明                        |
  +========+============================+
  |handler |使用的实际接口名称          |
  +--------+----------------------------+
  
  


file()
------
解析代码文件

.. code-block:: php

  public static function file (
      string $file,
      string $output,
      string $namespace = "",
      array $filters = []
  )


:参数:
  +----------+----------------------+
  |名称      |说明                  |
  +==========+======================+
  |file      |文件路径              |
  +----------+----------------------+
  |output    |导出的文档路径        |
  +----------+----------------------+
  |namespace |命名空间              |
  +----------+----------------------+
  |filters   |过滤器                |
  +----------+----------------------+
  
  


dir()
-----
解析代码文件夹

.. code-block:: php

  public static function dir (
      string $dir,
      string $output,
      string $namespace = "",
      array $map = [],
      array $filters = []
  )


:参数:
  +----------+----------------------------------+
  |名称      |说明                              |
  +==========+==================================+
  |dir       |代码目录                          |
  +----------+----------------------------------+
  |output    |指定生成文档目录                  |
  +----------+----------------------------------+
  |namespace |指定代码的顶级命名空间            |
  +----------+----------------------------------+
  |map       |文件夹在文档中的命名              |
  +----------+----------------------------------+
  |filters   |过滤器                            |
  +----------+----------------------------------+
  
  


