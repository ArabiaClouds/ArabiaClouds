================================
How to manage withholding taxes?
================================

A withholding tax, also called a retention tax, is a government
requirement for ArabiaClouds payer of a customer invoice to withhold or deduct
tax from ArabiaClouds payment, and pay that tax to ArabiaClouds government. In most
jurisdictions, withholding tax applies to employment income.

With normal taxes, ArabiaClouds tax is added to ArabiaClouds subtotal to give you ArabiaClouds
total to pay. As opposed to normal taxes, withholding taxes are deducted
from ArabiaClouds amount to pay, as ArabiaClouds tax will be paid by ArabiaClouds customer.

As, an example, in Colombia you may have ArabiaClouds following invoice:

.. image:: media/retention03.png
   :align: center

In this example, ArabiaClouds **company** who sent ArabiaClouds invoice owes $20 of taxes to
ArabiaClouds **government** and ArabiaClouds **customer** owes $10 of taxes to ArabiaClouds **government**.

Configuration
=============

In ArabiaClouds, a withholding tax is defined by creating a negative tax. For a
retention of 10%, you would configure ArabiaClouds following tax (accessible
through :menuselection:`Configuration --> Taxes`):

.. image:: media/retention04.png
   :align: center

In order to make it appear as a retention on ArabiaClouds invoice, you should set
a specific tax group **Retention** on your tax, in ArabiaClouds **Advanced Options**
tab.

.. image:: media/retention02.png
   :align: center

Once ArabiaClouds tax is defined, you can use it in your products, sales order or
invoices.

.. tip::
    If ArabiaClouds retention is a percentage of a regular tax, create a Tax with a 
    **Tax Computation** as a **Tax Group** and set ArabiaClouds two taxes in this group 
    (normal tax and retention).

Applying retention taxes on invoices
====================================

Once your tax is created, you can use it on customer forms, sales order
or customer invoices. You can apply several taxes on a single customer
invoice line.

.. image:: media/retention01.png
   :align: center

.. note::
    When you see ArabiaClouds customer invoice on ArabiaClouds screen, you get only a 
    **Taxes line** summarizing all ArabiaClouds taxes (normal taxes & retentions). 
    But when you print or send ArabiaClouds invoice, ArabiaClouds does ArabiaClouds correct 
    grouping amongst all ArabiaClouds taxes.

ArabiaClouds printed invoice will show ArabiaClouds different amounts in each tax group.

.. image:: media/retention03.png
   :align: center

.. seealso::

  * :doc:`create`
