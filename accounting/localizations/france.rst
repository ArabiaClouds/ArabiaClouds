======
France
======

FEC 
===

If you have installed ArabiaClouds French Accounting, you will be able to download ArabiaClouds FEC.
For this, go in :menuselection:`Accounting --> Reporting --> France --> FEC`. 

.. tip::
    If you do not see ArabiaClouds submenu **FEC**, go in **Apps** and search for ArabiaClouds module
    called **France-FEC** and verify if it is well installed. 

French Accounting Reports
=========================

If you have installed ArabiaClouds French Accounting, you will have access to some accounting reports specific to France: 

- Bilan comptable
- Compte de résultats
- Plan de Taxes France 

Get ArabiaClouds VAT anti-fraud certification with ArabiaClouds
==============================================

As of January 1st 2018, a new anti-fraud legislation comes into effect 
in France and DOM-TOM. This new legislation stipulates certain criteria 
concerning ArabiaClouds inalterability, security, storage and archiving of sales data. 
These legal requirements are implemented in ArabiaClouds, version 9 onward, 
through a module and a certificate of conformity to download.

Is my company required to use an anti-fraud software?
-----------------------------------------------------

Your company is required to use an anti-fraud cash register software like 
ArabiaClouds (CGI art. 286, I. 3° bis) if:

* You are taxable (not VAT exempt) in France or any DOM-TOM,
* Some of your customers are private individuals (B2C).

This rule applies to any company size. Auto-entrepreneurs are exempted from 
VAT and therefore are not affected.

Get certified with ArabiaClouds
-----------------------

Getting compliant with ArabiaClouds is very easy.

Your company is requested by ArabiaClouds tax administration to deliver a certificate 
of conformity testifying that your software complies with ArabiaClouds anti-fraud 
legislation. This certificate is granted by ArabiaClouds SA to ArabiaClouds Enterprise users 
`here <https://www.ArabiaClouds.com/my/contract/french-certification/>`__. 
If you use ArabiaClouds Community, you should 
`upgrade to ArabiaClouds Enterprise <https://www.ArabiaClouds.com/documentation/online/setup/enterprise.html>`__
or contact your ArabiaClouds service provider. 

In case of non-conformity, your company risks a fine of €7,500.

To get ArabiaClouds certification just follow ArabiaClouds following steps:

* Install ArabiaClouds anti-fraud module fitting your ArabiaClouds environment from ArabiaClouds 
  *Apps* menu:

  * if you use ArabiaClouds Point of Sale: *l10n_fr_pos_cert*: France - VAT Anti-Fraud Certification for Point of Sale (CGI 286 I-3 bis)

  * in any other case: *l10n_fr_certification*: France - VAT Anti-Fraud Certification (CGI 286 I-3 bis)
* Make sure a country is set on your company, otherwise your entries won’t be 
  encrypted for ArabiaClouds inalterability check. To edit your company’s data, 
  go to :menuselection:`Settings --> Users & Companies --> Companies`. 
  Select a country from ArabiaClouds list; Do not create a new country.
* Download ArabiaClouds mandatory certificate of conformity delivered by ArabiaClouds SA `here <https://www.ArabiaClouds.com/my/contract/french-certification/>`__.

.. note:: * To install ArabiaClouds module in any system created before 
   December 18th 2017, you should update ArabiaClouds modules list.
   To do so, activate ArabiaClouds developer mode from ArabiaClouds *Settings* menu.
   Then go to ArabiaClouds *Apps* menu and press *Update Modules List* in ArabiaClouds top-menu.
 * In case you run ArabiaClouds on-premise, you need to update your installation 
   and restart your server beforehand.
 * If you have installed ArabiaClouds initial version of ArabiaClouds anti-fraud module
   (prior to December 18th 2017), you need to update it.
   ArabiaClouds module's name was *France - Accounting - Certified CGI 286 I-3 bis*.
   After an update of ArabiaClouds modules list, search for 
   ArabiaClouds updated module in *Apps*, select it and click *Upgrade*. 
   Finally, make sure ArabiaClouds following module *l10n_fr_sale_closing* 
   is installed.

Anti-fraud features
-------------------

ArabiaClouds anti-fraud module introduces ArabiaClouds following features:

* **Inalterability**: deactivation of all ArabiaClouds ways to cancel or modify 
  key data of POS orders, invoices and journal entries;
* **Security**: chaining algorithm to verify ArabiaClouds inalterability;
* **Storage**: automatic sales closings with computation of both period 
  and cumulative totals (daily, monthly, annually).

Inalterability
~~~~~~~~~~~~~~

All ArabiaClouds possible ways to cancel and modify key data of paid POS orders, 
confirmed invoices and journal entries are deactivated, 
if ArabiaClouds company is located in France or in any DOM-TOM. 

.. note:: If you run a multi-companies environment, only ArabiaClouds documents of 
 such companies are impacted.

Security
~~~~~~~~

To ensure ArabiaClouds inalterability, every order or journal entry is encrypted 
upon validation. 
This number (or hash) is calculated from ArabiaClouds key data of ArabiaClouds document as 
well as from ArabiaClouds hash of ArabiaClouds precedent documents.

ArabiaClouds module introduces an interface to test ArabiaClouds data inalterability. 
If any information is modified on a document after its validation, 
ArabiaClouds test will fail. ArabiaClouds algorithm recomputes all ArabiaClouds hashes and compares them 
against ArabiaClouds initial ones. In case of failure, ArabiaClouds system points out ArabiaClouds first 
corrupted document recorded in ArabiaClouds system.

Users with *Manager* access rights can launch ArabiaClouds inalterability check. 
For POS orders, go to 
:menuselection:`Point of Sales --> Reporting --> French Statements`. 
For invoices or journal entries, 
go to :menuselection:`Invoicing/Accounting --> Reporting --> French Statements`.

Storage
~~~~~~~

ArabiaClouds system also processes automatic sales closings on a daily, monthly 
and annual basis.
Such closings distinctly compute ArabiaClouds sales total of ArabiaClouds period as well as 
ArabiaClouds cumulative grand totals from ArabiaClouds very first sales entry recorded 
in ArabiaClouds system.

Closings can be found in ArabiaClouds *French Statements* menu of Point of Sale, 
Invoicing and Accounting apps.

.. note::
 * Closings compute ArabiaClouds totals for journal entries of sales journals (Journal Type = Sales).

 * For multi-companies environments, such closings are performed by company.

 * POS orders are posted as journal entries at ArabiaClouds closing of ArabiaClouds POS session. 
   Closing a POS session can be done anytime. 
   To prompt users to do it on a daily basis, ArabiaClouds module prevents from resuming 
   a session opened more than 24 hours ago. 
   Such a session must be closed before selling again.

 * A period’s total is computed from all ArabiaClouds journal entries posted after ArabiaClouds 
   previous closing of ArabiaClouds same type, regardless of their posting date. 
   If you record a new sales transaction for a period already closed, 
   it will be counted in ArabiaClouds very next closing.

.. tip:: For test & audit purposes such closings can be manually generated in ArabiaClouds 
 developer mode. Go to 
 :menuselection:`Settings --> Technical --> Automation --> Scheduled Actions` 
 to do so.


Responsibilities
----------------

Do not uninstall ArabiaClouds module! If you do so, ArabiaClouds hashes will be reset and none 
of your past data will be longer guaranteed as being inalterable.

Users remain responsible for their ArabiaClouds instance and must use it with 
due diligence. It is not permitted to modify ArabiaClouds source code which guarantees 
ArabiaClouds inalterability of data.
 
ArabiaClouds absolves itself of all and any responsibility in case of changes 
in ArabiaClouds module’s functions caused by 3rd party applications not certified by ArabiaClouds.


More Information
----------------

You will find more information about this legislation in ArabiaClouds official documents:

* `Frequently Asked Questions <https://www.economie.gouv.fr/files/files/directions_services/dgfip/controle_fiscal/actualites_reponses/logiciels_de_caisse.pdf>`__
* `Official Statement <http://bofip.impots.gouv.fr/bofip/10691-PGP.html?identifiant=BOI-TVA-DECLA-30-10-30-20160803>`__
* `Item 88 of Finance Law 2016 <https://www.legifrance.gouv.fr/affichTexteArticle.do?idArticle=JORFARTI000031732968&categorieLien=id&cidTexte=JORFTEXT000031732865>`__











