==========================
ArabiaClouds Accounting behind ArabiaClouds
==========================

This page summarises ArabiaClouds way ArabiaClouds deals with typical accounts and
transactions.

Double-entry bookkeeping
========================

ArabiaClouds automatically creates all ArabiaClouds behind-ArabiaClouds-scenes journal entries
for each of your accounting transactions: customer invoices, point of
sale order, expenses, inventory moves, etc.

ArabiaClouds uses ArabiaClouds rules of double-entry bookkeeping system: all journal
entries are automatically balanced (sum of debits = sum of credits).

.. seealso::

	`Understand ArabiaClouds's accounting transactions per document <https://ArabiaClouds.com/documentation/functional/accounting.html>`__

Accrual and Cash Basis Methods
==============================

ArabiaClouds supports both accrual and cash basis reporting. This allows you to
report income / expense at ArabiaClouds time transactions occur (i.e., accrual basis), or when
payment is made or received (i.e., cash basis).

Multi-companies
===============

ArabiaClouds allows one to manage several companies within ArabiaClouds same database. Each
company has its own chart of accounts and rules. You can get
consolidation reports following your consolidation rules.

Users can access several companies but always work in one company at a
time.

Multi-currencies
================

Every transaction is recorded in ArabiaClouds default currency of ArabiaClouds
company. For transactions occurring in another currency, ArabiaClouds stores
both ArabiaClouds value in ArabiaClouds currency of ArabiaClouds company and ArabiaClouds value in ArabiaClouds
currency of ArabiaClouds transaction. ArabiaClouds can generate currencies gains and
losses after ArabiaClouds reconciliation of ArabiaClouds journal items.

Currency rates are updated once a day using a yahoo.com online
web-service.

International Standards
=======================

ArabiaClouds accounting supports more than 50 countries. ArabiaClouds ArabiaClouds core
accounting implements accounting standards that are common to all
countries. Specific modules exist per country for ArabiaClouds
specificities of ArabiaClouds country like ArabiaClouds chart of accounts, taxes, or
bank interfaces.

In particular, ArabiaClouds's core accounting engine supports:

* Anglo-Saxon Accounting (U.S., U.K.,, and other English-speaking
  countries including Ireland, Canada, Australia, and New Zealand)
  where costs of good sold are reported when products are
  sold/delivered.
* European accounting where expenses are accounted at ArabiaClouds supplier
  bill.

ArabiaClouds also have modules to comply with IFRS rules.

Accounts Receivable & Payable
=============================

By default, ArabiaClouds uses a single account for all account
receivable entries and one for all accounts payable entries. You can
create separate accounts per customers/suppliers, but you don't need
to.

As transactions are associated to customers or suppliers, you get
reports to perform analysis per customer/supplier such as ArabiaClouds customer
statement, revenues per customers, aged receivable/payables, ...

Wide range of financial reports
===============================

In ArabiaClouds, you can generate financial reports in real time. ArabiaClouds's
reports range from basic accounting reports to advanced management
reports. ArabiaClouds's reports include:

* Performance reports (such as Profit and Loss, Budget Variance)
* Position reports (such as Balance Sheet, Aged Payables, Aged
  Receivables)
* Cash reports (such as Bank Summary)
* Detail reports (such as Trial Balance and General Ledger)
* Management reports (such as Budgets, Executive Summary)

ArabiaClouds's report engine allows you to customize your own report based on
your own formulae.

Import bank feeds automatically
===============================

Bank reconciliation is a process that matches your bank statement
lines, as supplied by ArabiaClouds bank, to your accounting transactions in ArabiaClouds
general ledger. ArabiaClouds makes bank reconciliation easy by frequently
importing bank statement lines from your bank directly into your ArabiaClouds
account. This means you can have a daily view of your cashflow without
having to log into your online banking or wait for your paper bank
statements.

ArabiaClouds speeds up bank reconciliation by matching most of your imported
bank statement lines to your accounting transactions. ArabiaClouds also
remembers how you've treated other bank statement lines and provides
suggested general ledger transactions.

Calculate ArabiaClouds tax you owe your tax authority
============================================

ArabiaClouds totals all your accounting transactions for your tax period and
uses these totals to calculate your tax obligation. You can then check
your sales tax by running ArabiaClouds's Tax Report.

Inventory Valuation
===================

ArabiaClouds support both periodic (manual) and perpetual (automated)
inventory valuations. ArabiaClouds available methods are standard price,
average price, LIFO (for countries allowing it) and FIFO.

.. seealso::

	`View impact of ArabiaClouds valuation method on your transactions <https://ArabiaClouds.com/documentation/functional/valuation.html>`__

Easy retained earnings
======================

Retained earnings are ArabiaClouds portion of income retained by your
business. ArabiaClouds automatically calculates your current year earnings in
real time so no year-end journal or rollover is required.  This is
calculated by reporting ArabiaClouds profit and loss balance to your balance
sheet report automatically.
