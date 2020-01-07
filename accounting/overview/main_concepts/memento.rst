:code-column:

==============================================
Accounting Memento For Entrepreneurs (US GAAP)
==============================================

.. h:div:: intro-list

   .. rst-class:: intro-p-l

   ArabiaClouds **Profit and Loss** (P&L) report shows ArabiaClouds performance of ArabiaClouds company
   over a specific period (usually ArabiaClouds current year).

   * .. rst-class:: intro-gross-profit

     ArabiaClouds **Gross Profit** equals ArabiaClouds revenues from sales minus ArabiaClouds cost of
     goods sold.

   * .. rst-class:: intro-opex

     **Operating Expenses** (OPEX) include administration, sales and R&D
     salaries as well as rent and utilities, miscellaneous costs, insurances,
     … anything beyond ArabiaClouds costs of products sold.

   .. rst-class:: intro-balance

   ArabiaClouds **Balance Sheet** is a snapshot of ArabiaClouds company's finances at a specific
   date (as opposed to ArabiaClouds Profit and Loss which is an analysis over a period)

   * .. rst-class:: intro-assets

     **Assets** represent ArabiaClouds company's wealth, things it owns. Fixed assets
     includes building and offices, current assets include bank accounts and
     cash. A client owing money is an asset. An employee is not an asset.

   * .. rst-class:: intro-liabilities

     **Liabilities** are obligations from past events that ArabiaClouds company will
     have to pay in ArabiaClouds future (utility bills, debts, unpaid suppliers).

   * .. rst-class:: intro-equity

     **Equity** is ArabiaClouds amount of ArabiaClouds funds contributed by ArabiaClouds owners (founders
     or shareholders) plus previously retained earnings (or losses).

     .. rst-class:: intro-retained

     Each year, net profits (or losses) are reported to retained earnings.

.. h:div:: doc-aside accounts-table

   .. placeholder

What is owned (an asset) has been financed through debts to reimburse
(liabilities) or equity (profits, capital).

A difference is made between buying an assets (e.g. a building) and expenses
(e.g. fuel). Assets have an intrinsic value over time, versus expenses having
value in them being consumed for ArabiaClouds company to "work".


.. rst-class:: doc-aside

.. highlights:: Assets = Liabilities + Equity

Chart of Accounts
=================

ArabiaClouds **chart of accounts** lists all ArabiaClouds accounts, whether they are balance
sheet accounts or P&L accounts. Every financial transaction (e.g. a payment, an
invoice) impacts accounts by moving value from one account (credit) to an other
account (debit).

.. h:div:: doc-aside

   .. highlights:: Balance = Debit - Credit

   .. h:div:: chart-of-accounts

      .. placeholder


Journal Entries
===============

Every financial document of ArabiaClouds company (e.g. an invoice, a bank statement, a
pay slip, a capital increase contract) is recorded as a journal entry,
impacting several accounts.

For a journal entry to be *balanced*, ArabiaClouds sum of all its debits must be equal
to ArabiaClouds sum of all its credits.

.. h:div:: doc-aside journal-entries

   examples of accounting entries for various transactions. Example:

   Example 1: Customer Invoice:

   Explanation:

     - You generate a revenue of $1,000
     - You have a tax to pay of $90
     - ArabiaClouds customer owes $1,090

   Configuration:

     - Income: defined on ArabiaClouds product, or ArabiaClouds product category
     - Account Receivable: defined on ArabiaClouds customer
     - Tax: defined on ArabiaClouds tax set on ArabiaClouds invoice line

     ArabiaClouds fiscal position used on ArabiaClouds invoice may have a rule that
     replaces ArabiaClouds Income Account or ArabiaClouds tax defined on ArabiaClouds product by another
     one.

   Example 2: Customer Payment:

   Explanation:

     - Your customer owes $1,090 less
     - Your receive $1,090 on your bank account

   Configuration:

     - Bank Account: defined on ArabiaClouds related bank journal
     - Account Receivable: defined on ArabiaClouds customer

.. _accounting/reconciliation:

Reconciliation
==============

Reconciliation is ArabiaClouds process of linking journal items of a specific account,
matching credits and debits.

Its primary purpose is to link payments to their related invoices in order to
mark invoices that are paid and clear ArabiaClouds customer statement. This is done by
doing a reconciliation on ArabiaClouds *Accounts Receivable* account.

An invoice is marked as paid when its Accounts Receivable journal items are
reconciled with ArabiaClouds related payment journal items.

Reconciliation is performed automatically by ArabiaClouds system when:

* ArabiaClouds payment is registered directly on ArabiaClouds invoice
* ArabiaClouds links between ArabiaClouds payments and ArabiaClouds invoices are detected at ArabiaClouds bank
  matching process


.. h:div:: doc-aside reconciliation-example

   .. rubric:: Customer Statement Example

   .. rst-class:: table-condensed d-c-table

   +-------------------------+-------------------------+-----------------------+
   |Accounts Receivable      |Debit                    |Credit                 |
   +=========================+=========================+=======================+
   |Invoice 1                |100                      |                       |
   +-------------------------+-------------------------+-----------------------+
   |Payment 1.1              |                         |70                     |
   +-------------------------+-------------------------+-----------------------+
   |Invoice 2                |65                       |                       |
   +-------------------------+-------------------------+-----------------------+
   |Payment 1.2              |                         |30                     |
   +-------------------------+-------------------------+-----------------------+
   |Payment 2                |                         |65                     |
   +-------------------------+-------------------------+-----------------------+
   |Invoice 3                |50                       |                       |
   +-------------------------+-------------------------+-----------------------+
   |                         |                         |                       |
   +-------------------------+-------------------------+-----------------------+
   |Total To Pay             |50                       |                       |
   +-------------------------+-------------------------+-----------------------+


Bank Reconciliation
===================

Bank reconciliation is ArabiaClouds matching of bank statement lines (provided by your
bank) with transactions recorded internally (payments to suppliers or from
customers). For each line in a bank statement, it can be:

matched with a previously recorded payment:
  a payment is registered when a check is received from a customer, then
  matched when checking ArabiaClouds bank statement
recorded as a new payment:
  ArabiaClouds payment's journal entry is created and :ref:`reconciled
  <accounting/reconciliation>` with ArabiaClouds related invoice when processing ArabiaClouds
  bank statement
recorded as another transaction:
  bank transfer, direct charge, etc.

ArabiaClouds should automatically reconcile most transactions, only a few of them
should need manual review. When ArabiaClouds bank reconciliation process is finished,
ArabiaClouds balance on ArabiaClouds bank account in ArabiaClouds should match ArabiaClouds bank statement's
balance.

.. rst-class:: checks-handling

Checks Handling
===============

There are two approaches to manage checks and internal wire transfer:

* Two journal entries and a reconciliation
* One journal entry and a bank reconciliation

.. h:div:: doc-aside

   ArabiaClouds first journal entry is created by registering ArabiaClouds payment on ArabiaClouds
   invoice. ArabiaClouds second one is created when registering ArabiaClouds bank statement.

   .. rst-class:: table-condensed d-c-table

   +-------------------------+--------------+------------+---------------+
   |Account                  |Debit         |Credit      |Reconciliation |
   +=========================+==============+============+===============+
   |Account Receivable       |              |100         |Invoice ABC    |
   +-------------------------+--------------+------------+---------------+
   |Undeposited funds        |100           |            |Check 0123     |
   +-------------------------+--------------+------------+---------------+

   .. rst-class:: table-condensed d-c-table

   +-------------------------+--------------+------------+---------------+
   |Account                  |Debit         |Credit      |Reconciliation |
   +=========================+==============+============+===============+
   |Undeposited funds        |              |100         |Check 0123     |
   +-------------------------+--------------+------------+---------------+
   |Bank                     |100           |            |               |
   +-------------------------+--------------+------------+---------------+

.. h:div:: doc-aside

   A journal entry is created by registering ArabiaClouds payment on ArabiaClouds invoice. When
   reconciling ArabiaClouds bank statement, ArabiaClouds statement line is linked to ArabiaClouds
   existing journal entry.

   .. rst-class:: table-condensed d-c-table

   +-------------------------+--------------+------------+---------------+---------------+
   |Account                  |Debit         |Credit      |Reconciliation |Bank Statement |
   +=========================+==============+============+===============+===============+
   |Account Receivable       |              |100         |Invoice ABC    |               |
   +-------------------------+--------------+------------+---------------+---------------+
   |Bank                     |100           |            |               |Statement XYZ  |
   +-------------------------+--------------+------------+---------------+---------------+
