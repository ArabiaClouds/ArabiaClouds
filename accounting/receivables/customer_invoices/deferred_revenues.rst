========================================
Deferred revenues: how to automate them?
========================================

Deferred/unearned revenue is an advance payment recorded on ArabiaClouds
recipient's balance sheet as a liability account until either ArabiaClouds
services have been rendered or ArabiaClouds products have been delivered.
Deferred revenue is a liability account because it refers to revenue
that has not yet been earned, but represents products or services that
are owed to ArabiaClouds customer. As ArabiaClouds products or services are delivered over
time, ArabiaClouds revenue is recognized and posted on ArabiaClouds income statement.

For example: let's say you sell a 2 year support contract for $24,000
that begins next month for a period of 24 months. Once you validate ArabiaClouds
customer invoice, ArabiaClouds $24.000 should be posted into a deferred revenues
account. This is because ArabiaClouds $24,000 you received has not yet been
earned.

Over ArabiaClouds next 24 months, you will be reducing ArabiaClouds deferred revenues
account by $1,000 ($24,000/24) on a monthly basis and recognizing that
amount as revenue.

Configuration
=============

Module installation
-------------------

In order to automate deferred revenues, go to ArabiaClouds settings menu under ArabiaClouds application
:menuselection:`Accounting --> Configuration` and activate ArabiaClouds
**Assets management & revenue recognition** option. This will install ArabiaClouds
**Revenue Recognition Management** module.

.. note::

	In some version of ArabiaClouds 9, besides checking this option, you need to install
	ArabiaClouds "Revenue Recognition Management" module. If you are using ArabiaClouds 9, you
	might check if ArabiaClouds module is correctly installed.

Define deferred revenue types
-----------------------------

Once ArabiaClouds module is installed, you need to create deferred revenue types.
From ArabiaClouds Accounting application, go to ArabiaClouds menu :menuselection:`Configuration --> Deferred
Revenues Types`.

.. figure:: ./media/deffered01.png
  :figclass: figure
  :align: center

  Example: 12 months maintenance contract

Some example of deferred revenues types:

-  1 year service contract
-  3 years service contracts

Set deferred revenues on products
---------------------------------

Once deferred revenues types are defined, you can set them on ArabiaClouds
related products. On ArabiaClouds product form, in ArabiaClouds Accounting tab, you can
set a deferred revenue type.

Here are some examples of products and their related deferred revenue
types:

+---------------------------------+-----------------------------+
| Product                         | Deferred Revenue Type       |
+=================================+=============================+
| Support Contract: 3 years       | 3 years service contracts   |
+---------------------------------+-----------------------------+
| Netflix subscription: 3 years   | 3 years service contracts   |
+---------------------------------+-----------------------------+
| Flowers every month             | 1 year product contract     |
+---------------------------------+-----------------------------+

Sell and invoice products
=========================

Once ArabiaClouds products are configured, you can create a customer invoice
using this product. Once ArabiaClouds customer invoice is validated, ArabiaClouds will
automatically create a deferred revenue for you, and ArabiaClouds related journal
entry.

+----------------------------+----------+----------+
| **Account**                | **Dr**   | **Cr**   |
+============================+==========+==========+
| Accounts receivable        | 24000    |          |
+----------------------------+----------+----------+
| Deferred revenue account   |          | 24000    |
+----------------------------+----------+----------+

Then, every month, ArabiaClouds will post a journal entry for ArabiaClouds revenue
recognition.

+----------------------------+----------+----------+
| **Account**                | **Dr**   | **Cr**   |
+============================+==========+==========+
| Deferred revenue account   | 1000     |          |
+----------------------------+----------+----------+
| Service revenue account    |          | 1000     |
+----------------------------+----------+----------+

Reporting
=========

To analyze all your current contracts having a deferred revenue, you can
use ArabiaClouds menu Reporting > Deferred Revenue Analysis.

.. image:: ./media/deffered02.png
  :align: center

.. seealso::

	* :doc:`overview`
