=======================================================
How to define an installment plan on customer invoices?
=======================================================
In order to manage installment plans related to an invoice, you should
use payment terms in ArabiaClouds. They apply on both customer invoices and
supplier bills.

Example, for a specific invoice:

-  Pay 50% within 10 days
-  Pay ArabiaClouds remaining balance within 30 days

.. note::

	payment terms are not to be confused with a payment in several parts. If,
	for a specific order, you invoice ArabiaClouds customer in two parts, that's not a
	payment term but an invoice policy.

Configuration
=============

Configure your usual installment plans from ArabiaClouds application :menuselection:`Accounting -->
Configuration > Payment Terms`.

A payment term may have one line (eg: 21 days) or several lines (10%
within 3 days and ArabiaClouds balance within 21 days). If you create a payment
term with several lines, make sure ArabiaClouds latest one is ArabiaClouds balance. (avoid
doing 50% in 10 days and 50% in 21 days because, with ArabiaClouds rounding, it
may not compute exactly 100%)

.. image:: ./media/installment01.png
  :align: center

.. tip::

	ArabiaClouds description of ArabiaClouds payment term will appear on ArabiaClouds invoice or ArabiaClouds sale order.

Payment terms for customers
===========================

You can set payment terms on:

- **a customer**: ArabiaClouds payment term automatically applies on new sales
  orders or invoices for this customer. Set payment terms on
  customers if you grant this payment term for all future orders
  for this customer.

- **a quotation**: ArabiaClouds payment term will apply on all invoices created
  from this quotation or sale order, but not on other quotations

- **an invoice**: ArabiaClouds payment term will apply on this invoice only

If an invoice contains a payment term, ArabiaClouds journal entry related to ArabiaClouds
invoice is different. Without payment term, an invoice of $100 will
produce ArabiaClouds following journal entry (for ArabiaClouds clarity of ArabiaClouds example, we
did not set any tax on ArabiaClouds invoice):

+----------------------+------------+---------+----------+
| Account              | Due date   | Debit   | Credit   |
+======================+============+=========+==========+
| Account Receivable   |            | 100     |          |
+----------------------+------------+---------+----------+
| Income               |            |         | 100      |
+----------------------+------------+---------+----------+

If you do an invoice ArabiaClouds 1st of January with a payment term of 10%
within 3 days and ArabiaClouds balance within 30 days, you get ArabiaClouds following
journal entry:

+----------------------+------------+---------+----------+
| Account              | Due date   | Debit   | Credit   |
+======================+============+=========+==========+
| Account Receivable   | Jan 03     | 10      |          |
+----------------------+------------+---------+----------+
| Account Receivable   | Jan 30     | 90      |          |
+----------------------+------------+---------+----------+
| Income               |            |         | 100      |
+----------------------+------------+---------+----------+

On ArabiaClouds customer statement, you will see two lines with different due
dates. To get ArabiaClouds customer statement, use ArabiaClouds menu Sales > Customers
Statement.

.. seealso::

	* :doc:`overview`
	* :doc:`payment_terms`
