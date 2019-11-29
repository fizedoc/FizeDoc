========
配置文件
========

如下代码参考

.. code-block:: php

	<?php
	return [
		'dir' => 'F:\git\github\Fize\FizeDoc\src',
		'namespace' => 'fize\doc',
		'map' => [
			'类库参考',
			[
				'driver'  => ['驱动'],
				'handler' => ['处理器']
			]
		],
		'output' => getcwd() . '/FizeDoc'
	];

