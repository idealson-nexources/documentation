========
Products
========

Products can be created from the backend or the POS interface. To manage products from the backend,
go to :menuselection:`Point of Sale --> Products --> Products`. Click :guilabel:`New` to create a
product, or open an existing one to edit it. Update the fields as needed and ensure the
:guilabel:`Point of Sale` checkbox is enabled at the top of the form.

To create products from the POS interface, access the POS register, click the :icon:`fa-bars`
(:guilabel:`hamburger menu`) icon, then :guilabel:`Create Product`. Enter the product details in the
pop-up window and click :guilabel:`Save`. The product is immediately available in the register.

To update an existing product from the POS register, long-click a product to open the information
pop-up, and click :guilabel:`Edit`. Change the necessary product details and click :guilabel:`Save`
to return to the POS register.

POS product categories
======================

POS product categories are used to organize products in the POS register.

To manage POS categories, follow these steps:

#. Navigate to :menuselection:`Point of Sale --> Configuration --> PoS Product Categories`.
#. Click :guilabel:`New` to create a category or click an existing one to update it.
#. Classify and build a hierarchy between categories: Associate a category with a parent
   category by filling in the :guilabel:`Parent Category` field. A parent category groups one or
   more child categories (e.g., use `Drinks` to group `Hot beverages` and `Soft drinks`).

Once POS product categories are created, assign them to specific products:

#. Go to :menuselection:`Point of Sale --> Products --> Products` and open a product form.
#. Navigate to the :guilabel:`Point of Sale` tab and fill in the :guilabel:`Category` field with one
   or multiple POS categories.

To limit the categories displayed on the POS register, navigate to the :ref:`POS settings
<pos/use/settings>` and select the relevant categories in the :guilabel:`Restrict Categories` field
under the :guilabel:`Product & PoS categories` section.

.. _pos/products/combos:

Product combos
==============

A product combo consists of a set of items known as combo choices and offers combination options at
a special price.

.. _pos/products/combos/choices:

Combo choices creation
----------------------

To create the combo choices that will be added to the product combo, follow the next steps:

#. Go to :menuselection:`Point of Sale --> Products --> Combo Choices` and click :guilabel:`New`.
#. Enter a name for the combo choice.
#. Set the maximum selectable items for the combo using the :guilabel:`Maximum items` field.
#. Set the number of items included in the combo using the :guilabel:`Includes free` field.
#. Click :guilabel:`Add a line` under the :guilabel:`Options` section to add items that constitute
   the combo choices.

.. note::
   - The :guilabel:`Combo Price` field automatically calculates and displays the price for an extra
     item based on the price of the least expensive item in the selection.
   - Defining an :guilabel:`Extra Price` for an item alters the price of the product combo. The
     :guilabel:`Extra Price` differs from the :guilabel:`Combo Price`.

.. image:: products/combo-form.png
   :scale: 75%

.. _pos/products/combos/combo-creation:

Product combo creation
----------------------

To create a specific product to gather combo choices, follow the next steps:

#. Go to :menuselection:`Point of Sale --> Products --> Products` and click :guilabel:`New`.
#. Enter a product name.
#. Set the :guilabel:`Product Type` to :guilabel:`Combo` and select the relevant :guilabel:`Combo
   Choices`.
#. Add a :guilabel:`Sales Price`.
#. Optionally, click the :guilabel:`Point of Sale` tab to select the preferred :guilabel:`Category`.

.. note::
   The sales price of the combo product is fixed and does not vary based on the individual prices
   of included items or the quantity of items in the combo. The combo product price is only
   affected by the extra price optionally defined at the combo choice creation, or if a variant of
   one of the items has a specified extra price.

.. _pos/products/combos/application:

Practical application
---------------------

To use combos, follow these steps:

#. Open the POS register.
#. Click the desired combo, and select the preferred items.
#. Click :guilabel:`Add to order`.
#. Continue with the order process.
