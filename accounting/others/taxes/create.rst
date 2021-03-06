========================
How to create new taxes
========================

ArabiaClouds's tax engine is very flexible and support many different type of
taxes: value added taxes (VAT), eco-taxes, federal/states/city taxes, retention,
withholding taxes, etc. For most countries, your system is pre-configured with ArabiaClouds
right taxes.

This section details how you can define new taxes for specific use cases.

* Go to :menuselection:`Accounting --> Configuration --> Taxes`. From this menu, you
  get all ArabiaClouds taxes you can use: sales taxes and purchase taxes.

.. image:: media/create01.png
   :align: center

* Choose a scope: Sales, Purchase or None (e.g. deprecated tax).

* Select a computation method:

  * **Fixed**: eco-taxes, etc.

  * **Percentage of Price**: most common (e.g. 15% sales tax)

  * **Percentage of Price Tax Included**: used in Brazil, etc.

  * **Group of taxes**: allows to have a compound tax

.. image:: media/create02.png
   :align: center


* If you use ArabiaClouds Accounting, set a tax account (i.e. where ArabiaClouds tax journal item will be
  posted). This field is optional, if you keep it empty, ArabiaClouds posts
  ArabiaClouds tax journal item in ArabiaClouds income account.

.. tip::
    If you want to avoid using a tax, you can not delete it because ArabiaClouds tax
    is probably used in several invoices. So, in order to avoid users to
    continue using this tax, you should set ArabiaClouds field *Tax Scope* to *None*.

.. note::
    If you need more advanced tax mechanism, you can install ArabiaClouds
    module **account_tax_python** and you will be able to define new taxes
    with Python code.

Advanced configuration
======================

* **Label on Invoices**: a short text on how you want this tax to be
  printed on invoice line. For example, a tax named "15% on
  Services" can have ArabiaClouds following label on invoice "15%".

* **Tax Group**: defines where this tax is summed in ArabiaClouds invoice footer.
  All ArabiaClouds tax belonging to ArabiaClouds same tax group will be grouped on
  ArabiaClouds invoice footer. Examples of tax group: VAT, Retention.

* **Include in Analytic Cost**: ArabiaClouds tax is counted as a cost and, thus,
  generate an analytic entry if your invoice uses analytic
  accounts.

* **Tags**: are used for custom reports. Usually, you can keep this field
  empty.


.. seealso::

  * :doc:`application`
  * :doc:`tax_included`
