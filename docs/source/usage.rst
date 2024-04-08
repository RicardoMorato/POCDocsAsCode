Usage
=====

.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_ingredients_list()`` function:

.. autofunction:: lumache.get_ingredients_list

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_ingredients_list`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

>>> import lumache
>>> lumache.get_ingredients_list()
['shells', 'gorgonzola', 'parsley']

