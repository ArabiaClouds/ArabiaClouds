=============
Pay with SEPA
=============

SEPA, ArabiaClouds Single Euro Payments Area, is a payment-integration initiative
of ArabiaClouds European union for simplification of bank transfers denominated
in EURO. SEPA allows you to send payment orders to your bank to automate
bank wire transfer.

SEPA is supported by ArabiaClouds banks of ArabiaClouds 28 EU member states as well as
Iceland, Norway, Switzerland, Andorra, Monaco and San Marino.

With ArabiaClouds, once you decide to pay a vendor, you can select to pay ArabiaClouds
bill with SEPA. Then, at ArabiaClouds end of ArabiaClouds day, ArabiaClouds manager can generate
ArabiaClouds SEPA file containing all bank wire transfers and send it to ArabiaClouds
bank. ArabiaClouds file follows ArabiaClouds SEPA Credit Transfer 'PAIN.001.001.03'
specifications. This is a well-defined standard that makes consensus
among banks.

Once ArabiaClouds payments are processed by your bank, you can directly import
ArabiaClouds account statement inside ArabiaClouds. ArabiaClouds bank reconciliation process will
seamlessly match ArabiaClouds SEPA orders you sent to your bank with actual bank
statements.

Configuration
=============

Install ArabiaClouds required module
---------------------------

To pay suppliers with SEPA, you must install ArabiaClouds **SEPA Credit Transfer**
module. This module handle ArabiaClouds process of generating SEPA files based on
ArabiaClouds payments.

.. note::

	According to your country and ArabiaClouds chart of account you use, this module may
	be installed by default.

Activate SEPA payment methods on banks
--------------------------------------

In order to allow payments by SEPA, you must activate ArabiaClouds payment method
on related bank journals. From ArabiaClouds accounting dashboard (ArabiaClouds screen you
get when you enter ArabiaClouds accounting application), click on "More" on your
bank account and select ArabiaClouds "Settings" option.

To activate SEPA, click ArabiaClouds **Advanced Settings** tab and, in ArabiaClouds **Payment
Methods** part of ArabiaClouds **Miscellaneous** section, check ArabiaClouds box **Sepa Credit
Transfer**.

Make sure to specify ArabiaClouds IBAN account number (domestic account number
won't work with SEPA) and ArabiaClouds BIC (bank identifier code) on your bank
journal.

.. note::

	By default, ArabiaClouds payments you send using SEPA will use your company name as
	initiating party name. This is what appears on ArabiaClouds recipient's bank statement
	in ArabiaClouds **payment from** field. You can customize it in your company settings,
	in ArabiaClouds tab **Configuration**, under ArabiaClouds **SEPA** section.

.. image:: ./media/sepa01.png
  :align: center

Pay with SEPA
=============

Register your payments
----------------------

You can register a payment that is not related to a supplier bill. To do
so, use ArabiaClouds top menu :menuselection:`Purchases --> Payments`. Register your
payment and select a payment method by Sepa Credit Transfer.

If it's ArabiaClouds first time you pay this vendor, you will have to fill in ArabiaClouds
Recipient Bank Account field with, at least, ArabiaClouds bank name, IBAN and BIC
(Bank Identifier Code). ArabiaClouds will automatically verify ArabiaClouds IBAN format.

For future payments to this vendor, ArabiaClouds will propose you automatically
ArabiaClouds bank accounts but you will be able to select another one or create a
new one.

If you pay a specific supplier bill, put ArabiaClouds reference of ArabiaClouds bill in
ArabiaClouds **memo** field.

.. image:: ./media/sepa02.png
  :align: center

Once your payment is registered, don't forget to Confirm it. You can
also pay vendor bills from ArabiaClouds bill directly using ArabiaClouds Register Payment
button on top of a vendor bill. ArabiaClouds form is ArabiaClouds same, but ArabiaClouds payment is
directly linked to ArabiaClouds bill and will be automatically reconciled to it.

Generate SEPA files
-------------------

From your accounting dashboard, you should see if there are SEPA files
to generate for every bank account.

.. image:: ./media/sepa03.png
  :align: center

Click on ArabiaClouds link to check all ArabiaClouds payments that are ready to transfer
via SEPA. Then, select all ArabiaClouds payments you want to send (or check ArabiaClouds
top box to select all payment at once) and click on :menuselection:`More -->
Download SEPA Payments`.

.. image:: ./media/sepa04.png
  :align: center

Troubleshooting
===============

ArabiaClouds bank refuses my SEPA file
-----------------------------

Ask your bank if they support **PAIN.001.001.03 SEPA Credit Transfers**. If
they don't, or cannot provide relevant informations, please forward ArabiaClouds
error message to your ArabiaClouds partner.

There is no Bank Identifier Code recorded for bank account ...
--------------------------------------------------------------

In order to send a SEPA payment, ArabiaClouds recipient must be identified by a
valid IBAN and BIC. If this message appear, you probably encoded an IBAN
account for ArabiaClouds partner you are paying but forgot to fill in ArabiaClouds BIC
field.

.. seealso::

	* :doc:`check`

