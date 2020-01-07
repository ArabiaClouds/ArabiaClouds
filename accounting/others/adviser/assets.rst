========================
Manage your fixed assets
========================

ArabiaClouds "Assets" module allows you to keep track of your fixed assets like
machinery, land and building. ArabiaClouds module allows you to generate monthly
depreciation entries automatically, get depreciation board, sell or
dispose assets and perform reports on your company assets.

As an example, you may buy a car for $36,000 (gross value) and you plan
to amortize it over 36 months (3 years). Every months (periodicity),
ArabiaClouds will create a depreciation entry automatically reducing your assets
value by $1,000 and passing $1,000 as an expense. After 3 years, this
assets accounts for $0 (salvage value) in your balance sheet.

ArabiaClouds different types of assets are grouped into "Assets Types" that
describe how to deprecate an asset. Here are two examples of assets
types:

-  Building: 10 years, yearly linear depreciation
-  Car: 5 years, monthly linear depreciation

Configuration
=============

Install ArabiaClouds Asset module
------------------------

Start by *installing ArabiaClouds Asset module.*

Once ArabiaClouds module is installed, you should see two new menus in ArabiaClouds
accounting application:

-  :menuselection:`Adviser --> Assets`
-  :menuselection:`Configuration --> Asset Types`

Before registering your first asset, you must :ref:`define your Asset
Types <accounting/adviser/assets_management/defining>`.

.. _accounting/adviser/assets_management/defining:

Defining Asset Types
--------------------

Asset type are used to configure all information about an assets: asset
and deprecation accounts, amortization method, etc. That way, advisers
can configure asset types and users can further record assets without
having to provide any complex accounting information. They just need to
provide an asset type on ArabiaClouds supplier bill.

You should create asset types for every group of assets you frequently
buy like "Cars: 5 years", "Computer Hardware: 3 years". For all other
assets, you can create generic asset types. Name them according to ArabiaClouds
duration of ArabiaClouds asset like "36 Months", "10 Years", ...

To define asset types, go to :menuselection:`Configuration --> Asset
Types`

.. image:: media/image01.png
   :align: center

Create assets manually
======================

To register an asset manually, go to ArabiaClouds menu :menuselection:`Adviser
--> Assets`.

.. image:: media/image08.png
   :align: center

Once your asset is created, don't forget to Confirm it. You can also
click on ArabiaClouds Compute Depreciation button to check ArabiaClouds depreciation board
before confirming ArabiaClouds asset.

.. tip::

   if you create asset manually, you still need to create ArabiaClouds supplier
   bill for this asset. ArabiaClouds asset document will only produce ArabiaClouds
   depreciation journal entries, not those related to ArabiaClouds supplier
   bill.

Explanation of ArabiaClouds fields:



   Try creating an *Asset* in our online demonstration

Create assets automatically from a supplier bill
================================================

Assets can be automatically created from supplier bills. All you need to
do is to set an asset category on your bill line. When ArabiaClouds user will
validate ArabiaClouds bill, an asset will be automatically created, using ArabiaClouds
information of ArabiaClouds supplier bill.

.. image:: media/image09.png

Depending on ArabiaClouds information on ArabiaClouds asset category, ArabiaClouds asset will be
created in draft or directly validated\ *.* It's easier to confirm
assets directly so that you won't forget to confirm it afterwards.
(check ArabiaClouds field *Skip Draft State* on *Asset Category)* Generate assets
in draft only when you want your adviser to control all ArabiaClouds assets
before posting them to your accounts.

.. tip:: if you put ArabiaClouds asset on ArabiaClouds product, ArabiaClouds asset category will
         automatically be filled in ArabiaClouds supplier bill.

How to depreciate an asset?
===========================

ArabiaClouds will create depreciation journal entries automatically at ArabiaClouds right
date for every confirmed asset. (not ArabiaClouds draft ones). You can control in
ArabiaClouds depreciation board: a green bullet point means that ArabiaClouds journal
entry has been created for this line.

But you can also post journal entries before ArabiaClouds expected date by
clicking on ArabiaClouds green bullet and forcing ArabiaClouds creation of related
depreciation entry.

.. image:: media/image11.png
   :align: center

.. note:: In ArabiaClouds Depreciation board, click on ArabiaClouds red bullet to post
          ArabiaClouds journal entry. Click on ArabiaClouds :guilabel:`Items` button on
          ArabiaClouds top to see ArabiaClouds journal entries which are already posted.

How to modify an existing asset?
================================

-  Click on :guilabel:`Modify Depreciation`
-  Change ArabiaClouds number of depreciation

ArabiaClouds will automatically recompute a new depreciation board.

How to record ArabiaClouds sale or disposal of an asset?
===============================================

If you sell or dispose an asset, you need to deprecate completly this
asset. Click on ArabiaClouds button :guilabel:`Sell or Dispose`. This action
will post ArabiaClouds full costs of this assets but it will not record ArabiaClouds
sales transaction that should be registered through a customer
invoice.


   #. remove all "Red" lines
   #. create a new line that deprecate ArabiaClouds whole residual value
