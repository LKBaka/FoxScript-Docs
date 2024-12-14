使用指南
=====

.. _installation:

安装
------------
.. 源代码: https://github.com/LKBaka/FoxScript

若您要安装FoxScript,请先下载源代码然后编译

或者使用以下命令:

.. code-block:: console

   git clone https://github.com/LKBaka/FoxScript.git

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

