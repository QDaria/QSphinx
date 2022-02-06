Usage
=====

.. _installation:

Installation
------------

To use QDaria, first install it using pip:

.. code-block:: console

   (.venv) $ pip install qdaria

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``qdaria.get_random_ingredients()`` function:

.. py:function:: qdaria.get_random_ingredients(kind=None)

   Return a list of random ingredients as strings.

   :param kind: Optional "kind" of ingredients.
   :type kind: list[str] or None
   :return: The ingredients list.
   :rtype: list[str]


The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`qdaria.get_random_ingredients`
will raise an exception.

.. py:exception:: qdaria.InvalidKindError

   Raised if the kind is invalid.


.. py:function:: qdaria.get_random_ingredients(kind=None)

   Return a list of random ingredients as strings.

   :param kind: Optional "kind" of ingredients.
   :type kind: list[str] or None
   :raise qdaria.InvalidKindError: If the kind is invalid.
   :return: The ingredients list.
   :rtype: list[str]


>>> import qdaria
>>> qdaria.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']


def get_random_ingredients(kind=None):
    return ["eggs", "bacon", "spam"]

you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients


or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError