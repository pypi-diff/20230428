# Comparing `tmp/lockstep-sdk-2023.5.21.tar.gz` & `tmp/lockstep-sdk-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockstep-sdk-2023.5.21.tar", last modified: Tue Feb  7 20:15:08 2023, max compression
+gzip compressed data, was "lockstep-sdk-2023.7.7.tar", last modified: Thu Feb 16 16:16:59 2023, max compression
```

## Comparing `lockstep-sdk-2023.5.21.tar` & `lockstep-sdk-2023.7.7.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:15:08.312912 lockstep-sdk-2023.5.21/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-02-07 20:15:08.312912 lockstep-sdk-2023.5.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-07 20:15:08.312912 lockstep-sdk-2023.5.21/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:15:08.292912 lockstep-sdk-2023.5.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:15:08.292912 lockstep-sdk-2023.5.21/src/lockstep/
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:15:08.296912 lockstep-sdk-2023.5.21/src/lockstep/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/apikeys_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/appenrollments_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/applications_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/attachmentlinks_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/attachments_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/codedefinitions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/companies_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/contacts_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/creditmemosapplied_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/currencies_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/customfielddefinitions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/customfieldvalues_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/definitions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/featureflags_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/financialaccount_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/financialaccountbalancehistory_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/financialyearsettings_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/groupaccounts_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/invoiceaddresses_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/invoicehistory_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/invoicelines_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/invoices_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/leads_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/magiclinks_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/notes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17704 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/payments_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/paymentsapplied_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/profilesaccounting_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/profilesaccountingcontacts_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/profilescompanies_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/provisioning_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30372 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/reports_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/status_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/sync_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/transactions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/transcriptions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/useraccounts_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/userroles_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/webhookrules_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/clients/webhooks_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/fetch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/lockstep_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/lockstep_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:15:08.312912 lockstep-sdk-2023.5.21/src/lockstep/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilecontactmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilecontactresultmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilerequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/actionresultmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/agingmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/apagingheaderinfomodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/apheaderinfomodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/apikeymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/appenrollmentcustomfieldmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/appenrollmentmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/appenrollmentreconnectinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/applicationmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/aragingheaderinfomodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/arheaderinfomodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/atriskinvoicesummarymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/attachmentheaderinfomodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/attachmentlinkmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/attachmentmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/basecurrencysyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/batchsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/bulkcurrencyconversionmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/bulkdeleterequestmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/cashflowreportmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/codedefinitionmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/companydetailsmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/companydetailspaymentmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/companymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/companysyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/connectorinfomodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/contactmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/contactsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/countrymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/creditmemoappliedmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/creditmemoappliedsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/creditmemoinvoicemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/currencymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/currencyratemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/customersummarymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/customfielddefinitionmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/customfieldsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/customfieldvaluemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/dailypayableoutstandingreportmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/dailysalesoutstandingreportmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/deleteresult.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/developeraccountsubmitmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/dposummarygrouptotalmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/dposummarymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/erpmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/errorresult.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/featureflagsrequestmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/featureflagsresponsemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountbalancehistorymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountbalancehistorysyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialreportcellmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialreportmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialreportrowmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialyearsettingmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/financialyearsettingsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/groupaccountmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invitedatamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invitemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invitesubmitmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoiceaddressmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicehistorymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicelinemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicelinesyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicepaymentdetailmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicesummarymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicesummarymodelinvoicesummarytotalsmodelsummaryfetchresult.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicesummarytotalsmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/invoicesyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/leadmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/magiclinkmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/magiclinkstatusmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/notemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/payablescomingdueheadermodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/payablescomingduemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/payablescomingduewidgetmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/payablessummaryreportmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentappliedmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentappliedsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentdetailheadermodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentdetailmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentsummarymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentsummarymodelpaymentsummarytotalsmodelsummaryfetchresult.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentsummarytotalsmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/paymentsyncmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/publiccompanyprofilemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/riskratemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/statemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/statusmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/summaryagingtotalsmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/supportaccessmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/supportaccessrequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/syncentityresultmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/syncrequestmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/syncsubmitmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transactiondetailmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transactionmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transactionmodeltransactionsummarytotalmodelsummaryfetchresult.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transactionsummarytotalmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transcriptionrequestsubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transcriptionvalidationrequestitemmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transcriptionvalidationrequestmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transferownermodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/transferownersubmitmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/urimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/useraccountmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/userdataresponsemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/usergroupmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/userrolemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/vendorsummarymodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/viewboxsettingsmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/webhookhistorytablestoragemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/webhookmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-07 20:14:41.000000 lockstep-sdk-2023.5.21/src/lockstep/models/webhookrulemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 20:15:08.312912 lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-02-07 20:15:08.000000 lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-02-07 20:15:08.000000 lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 20:15:08.000000 lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-07 20:15:08.000000 lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-07 20:15:08.000000 lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:59.299888 lockstep-sdk-2023.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-02-16 16:16:59.299888 lockstep-sdk-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-16 16:16:59.299888 lockstep-sdk-2023.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:59.279888 lockstep-sdk-2023.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:59.279888 lockstep-sdk-2023.7.7/src/lockstep/
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:59.283888 lockstep-sdk-2023.7.7/src/lockstep/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/apikeys_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/appenrollments_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/applications_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/attachmentlinks_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/attachments_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/codedefinitions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/companies_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/contacts_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/creditmemosapplied_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/currencies_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/customfielddefinitions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/customfieldvalues_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/definitions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/featureflags_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/financialaccount_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/financialaccountbalancehistory_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/financialyearsettings_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/groupaccounts_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/invoiceaddresses_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/invoicehistory_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/invoicelines_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/invoices_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/leads_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/magiclinks_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/notes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17704 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/payments_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/paymentsapplied_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/profilesaccounting_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/profilesaccountingcontacts_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/profilescompanies_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/provisioning_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30372 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/reports_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/status_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/sync_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/transactions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/transcriptions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/useraccounts_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/userroles_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/webhookrules_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/clients/webhooks_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/fetch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/lockstep_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/lockstep_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:59.299888 lockstep-sdk-2023.7.7/src/lockstep/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilecontactmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilecontactresultmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilerequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/actionresultmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/agingmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/apagingheaderinfomodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/apheaderinfomodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/apikeymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/appenrollmentcustomfieldmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/appenrollmentmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/appenrollmentreconnectinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/applicationmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/aragingheaderinfomodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/arheaderinfomodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/atriskinvoicesummarymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/attachmentheaderinfomodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/attachmentlinkmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/attachmentmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/basecurrencysyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/batchsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/bulkcurrencyconversionmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/bulkdeleterequestmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/cashflowreportmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/codedefinitionmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/companydetailsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/companydetailspaymentmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/companymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/companysyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/connectorinfomodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/contactmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/contactsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/countrymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/creditmemoappliedmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/creditmemoappliedsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/creditmemoinvoicemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/currencymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/currencyratemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/customersummarymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/customfielddefinitionmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/customfieldsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/customfieldvaluemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/dailypayableoutstandingreportmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/dailysalesoutstandingreportmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/deleteresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/developeraccountsubmitmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/dposummarygrouptotalmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/dposummarymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/erpmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/errorresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/featureflagsrequestmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/featureflagsresponsemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountbalancehistorymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountbalancehistorysyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialreportcellmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialreportmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialreportrowmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialyearsettingmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/financialyearsettingsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/groupaccountmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invitedatamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invitemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invitesubmitmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoiceaddressmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicehistorymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicelinemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicelinesyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicepaymentdetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicesummarymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicesummarymodelinvoicesummarytotalsmodelsummaryfetchresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicesummarytotalsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/invoicesyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/leadmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/magiclinkmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/magiclinkstatusmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/notemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/payablescomingdueheadermodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/payablescomingduemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/payablescomingduewidgetmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/payablessummaryreportmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentappliedmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentappliedsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentdetailheadermodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentdetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentsummarymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentsummarymodelpaymentsummarytotalsmodelsummaryfetchresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentsummarytotalsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/paymentsyncmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/publiccompanyprofilemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/riskratemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/statemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/statusmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/summaryagingtotalsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/supportaccessmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/supportaccessrequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/syncentityresultmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/syncrequestmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/syncsubmitmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transactiondetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transactionmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transactionmodeltransactionsummarytotalmodelsummaryfetchresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transactionsummarytotalmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transcriptionrequestsubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transcriptionvalidationrequestitemmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transcriptionvalidationrequestmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transferownermodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/transferownersubmitmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/urimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/useraccountmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/userdataresponsemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/usergroupmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/userrolemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/vendorsummarymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/viewboxsettingsmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/webhookhistorytablestoragemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/webhookmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-16 16:16:22.000000 lockstep-sdk-2023.7.7/src/lockstep/models/webhookrulemodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 16:16:59.299888 lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-02-16 16:16:59.000000 lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-02-16 16:16:59.000000 lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 16:16:59.000000 lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-16 16:16:59.000000 lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-16 16:16:59.000000 lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/top_level.txt
```

### Comparing `lockstep-sdk-2023.5.21/LICENSE` & `lockstep-sdk-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/PKG-INFO` & `lockstep-sdk-2023.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockstep-sdk
-Version: 2023.5.21
+Version: 2023.7.7
 Summary: Lockstep Platform SDK for Python
 Home-page: https://github.com/Lockstep-Network/lockstep-sdk-python
 Author: Lockstep
 Author-email: developer@lockstep.io
 Project-URL: Bug Tracker, https://github.com/Lockstep-Network/lockstep-sdk-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lockstep-sdk-2023.5.21/README.md` & `lockstep-sdk-2023.7.7/README.md`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/setup.cfg` & `lockstep-sdk-2023.7.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lockstep-sdk
-version = 2023.5.21
+version = 2023.7.7
 author = Lockstep
 author_email = developer@lockstep.io
 description = Lockstep Platform SDK for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Lockstep-Network/lockstep-sdk-python
 project_urls =
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/__init__.py` & `lockstep-sdk-2023.7.7/src/lockstep/__init__.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/apikeys_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/apikeys_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/appenrollments_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/appenrollments_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/applications_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/applications_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/attachmentlinks_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/attachmentlinks_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/attachments_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/attachments_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/codedefinitions_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/codedefinitions_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/companies_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/companies_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/contacts_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/contacts_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/creditmemosapplied_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/creditmemosapplied_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/currencies_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/currencies_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/customfielddefinitions_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/customfielddefinitions_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/customfieldvalues_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/customfieldvalues_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/definitions_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/definitions_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/featureflags_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/featureflags_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/financialaccount_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/financialaccount_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/financialaccountbalancehistory_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/financialaccountbalancehistory_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/financialyearsettings_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/financialyearsettings_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/groupaccounts_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/groupaccounts_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/invoiceaddresses_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/invoiceaddresses_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/invoicehistory_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/invoicehistory_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/invoicelines_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/invoicelines_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/invoices_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/invoices_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/leads_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/leads_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/magiclinks_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/magiclinks_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/notes_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/notes_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/payments_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/payments_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/paymentsapplied_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/paymentsapplied_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/profilesaccounting_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/profilesaccounting_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/profilesaccountingcontacts_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/profilesaccountingcontacts_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,46 +88,14 @@
         path = "/api/v1/profiles/accounting/contacts"
         result = self.client.send_request("POST", path, body, {}, None)
         if result.status_code >= 200 and result.status_code < 300:
             return LockstepResponse(True, result.status_code, list[AccountingProfileContactModel](**result.json()), None)
         else:
             return LockstepResponse(False, result.status_code, None, ErrorResult(**result.json()))
 
-    def update_accounting_profile_contact(self, id: str, contactId: str) -> LockstepResponse[AccountingProfileContactModel]:
-        """
-        Updates an accounting profile contact that matches the specified
-        id with the requested information.
-
-        The PATCH method allows you to change specific values on the
-        object while leaving other values alone. As input you should
-        supply a list of field names and new values. If you do not
-        provide the name of a field, that field will remain unchanged.
-        This allows you to ensure that you are only updating the
-        specific fields desired.
-
-        An Accounting Profile Contact has a link to a Contact that is
-        associated with your company's Accounting Profile. A profile has
-        one primary contact and any number of secondary contacts.
-
-        Parameters
-        ----------
-        id : str
-            The unique Lockstep Platform ID number of the Accounting
-            Profile Contact to update
-        contactId : str
-            The ID of the contact to link to this Accounting Profile
-            Contact
-        """
-        path = f"/api/v1/profiles/accounting/contacts/{id}/{contactId}"
-        result = self.client.send_request("PATCH", path, None, {}, None)
-        if result.status_code >= 200 and result.status_code < 300:
-            return LockstepResponse(True, result.status_code, AccountingProfileContactModel(**result.json()), None)
-        else:
-            return LockstepResponse(False, result.status_code, None, ErrorResult(**result.json()))
-
     def query_accounting_profile_contacts(self, filter: str, include: str, order: str, pageSize: int, pageNumber: int) -> LockstepResponse[FetchResult[AccountingProfileContactModel]]:
         """
         Queries Accounting Profile Contacts for this account using the
         specified filtering, sorting, nested fetch, and pagination rules
         requested.
 
         More information on querying can be found on the [Searchlight
@@ -206,26 +174,27 @@
         if result.status_code >= 200 and result.status_code < 300:
             return LockstepResponse(True, result.status_code, FetchResult[AccountingProfileContactResultModel](**result.json()), None)
         else:
             return LockstepResponse(False, result.status_code, None, ErrorResult(**result.json()))
 
     def set_secondary_contact_as_primary(self, id: str) -> LockstepResponse[AccountingProfileContactModel]:
         """
-        Updates an accounting profile contact that matches the specified
-        id with the primary contact attached to the accounting profile
+        Reverses the isPrimary fields on the primary and secondary
+        contact to reflect a swap and returns the new primary accounting
+        profile contact model.
 
         An Accounting Profile Contact has a link to a Contact that is
         associated with your company's Accounting Profile. A profile has
         one primary contact and any number of secondary contacts.
 
         Parameters
         ----------
         id : str
             The unique Lockstep Platform ID number of the Accounting
-            Profile Contact to update
+            Profile Contact to set as primary
         """
         path = f"/api/v1/profiles/accounting/contacts/{id}/primary"
         result = self.client.send_request("PATCH", path, None, {}, None)
         if result.status_code >= 200 and result.status_code < 300:
             return LockstepResponse(True, result.status_code, AccountingProfileContactModel(**result.json()), None)
         else:
             return LockstepResponse(False, result.status_code, None, ErrorResult(**result.json()))
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/profilescompanies_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/profilescompanies_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/provisioning_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/provisioning_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/reports_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/reports_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/status_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/status_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/sync_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/sync_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         path = "/api/v1/Sync/batch"
         result = self.client.send_request("POST", path, body, {}, None)
         if result.status_code >= 200 and result.status_code < 300:
             return LockstepResponse(True, result.status_code, SyncRequestModel(**result.json()), None)
         else:
             return LockstepResponse(False, result.status_code, None, ErrorResult(**result.json()))
 
-    def upload_sync_file(self, filename: str) -> LockstepResponse[SyncRequestModel]:
+    def upload_sync_file(self, appEnrollmentId: str, isFullSync: bool, filename: str) -> LockstepResponse[SyncRequestModel]:
         """
         Requests a new Sync task from a ZIP file you provide. This ZIP
         file can contain one or more files with data from the customer's
         platform. Individual files can be in the format CSV or JSONL
         (JSON with Lines).
 
         A Sync task represents an action performed by an Application for
@@ -93,19 +93,25 @@
         tasks as part of their capabilities. Sync tasks are executed in
         the background and will continue running after they are created.
         Use one of the creation APIs to request execution of a task. To
         check on the progress of the task, call GetSync or QuerySync.
 
         Parameters
         ----------
+        appEnrollmentId : str
+            The optional existing app enrollment to associate with the
+            data in the zip file.
+        isFullSync : bool
+            True if this is a full sync, false if this is a partial
+            sync. Defaults to false.
         filename : str
             The full path of a file to upload to the API
         """
         path = "/api/v1/Sync/zip"
-        result = self.client.send_request("POST", path, None, {}, filename)
+        result = self.client.send_request("POST", path, None, {"appEnrollmentId": appEnrollmentId, "isFullSync": isFullSync}, filename)
         if result.status_code >= 200 and result.status_code < 300:
             return LockstepResponse(True, result.status_code, SyncRequestModel(**result.json()), None)
         else:
             return LockstepResponse(False, result.status_code, None, ErrorResult(**result.json()))
 
     def update_sync(self, id: str, body: object) -> LockstepResponse[SyncRequestModel]:
         """
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/transactions_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/transactions_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/transcriptions_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/transcriptions_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/useraccounts_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/useraccounts_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/userroles_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/userroles_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/webhookrules_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/webhookrules_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/clients/webhooks_client.py` & `lockstep-sdk-2023.7.7/src/lockstep/clients/webhooks_client.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/fetch_result.py` & `lockstep-sdk-2023.7.7/src/lockstep/fetch_result.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/lockstep_api.py` & `lockstep-sdk-2023.7.7/src/lockstep/lockstep_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # For the full copyright and license information, please view the LICENSE
 # file that was distributed with this source code.
 #
 # @author     Lockstep Network <support@lockstep.io>
 #             
 # @copyright  2021-2023 Lockstep, Inc.
-# @version    2023.5.21
+# @version    2023.7.7
 # @link       https://github.com/Lockstep-Network/lockstep-sdk-python
 #
 
 import platform
 import requests
 import typing
 import urllib.parse
@@ -124,15 +124,15 @@
         self.webhooks = WebhooksClient(self)
         self.serverUrl = env
         if env == "sbx":
             self.serverUrl = "https://api.sbx.lockstep.io/"
         if env == "prd":
             self.serverUrl = "https://api.lockstep.io/"
         self.sdkName = "Python"
-        self.sdkVersion = "2023.5.21"
+        self.sdkVersion = "2023.7.7"
         self.machineName = platform.uname().node
         self.applicationName = appname
         self.apiKey = None
         self.bearerToken = None
     
     def with_api_key(self, apiKey: str):
         """Configure this API client to use API Key authentication
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/lockstep_response.py` & `lockstep-sdk-2023.7.7/src/lockstep/lockstep_response.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilecontactmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilecontactmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilecontactresultmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilecontactresultmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/accountingprofilerequest.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/accountingprofilerequest.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/actionresultmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/actionresultmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/agingmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/agingmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/apagingheaderinfomodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/apagingheaderinfomodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/apheaderinfomodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/apheaderinfomodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/apikeymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/apikeymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/appenrollmentcustomfieldmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/appenrollmentcustomfieldmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/appenrollmentmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/appenrollmentmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/appenrollmentreconnectinfo.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/appenrollmentreconnectinfo.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/applicationmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/applicationmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/aragingheaderinfomodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/aragingheaderinfomodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/arheaderinfomodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/arheaderinfomodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/atriskinvoicesummarymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/atriskinvoicesummarymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/attachmentheaderinfomodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/attachmentheaderinfomodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/attachmentlinkmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/attachmentlinkmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/attachmentmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/attachmentmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/basecurrencysyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/basecurrencysyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/batchsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/batchsyncmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     permits either a complete data file or a partial / delta data file.
     Lockstep recommends using a sliding time window to avoid the risk of
     clock skew errors that might accidentally omit records. Best
     practice is to run a Sync process daily, and to export all data that
     has changed in the past 48 hours.
     """
 
+    appEnrollmentId: str | None = None
+    isFullSync: bool | None = None
     companies: list[CompanySyncModel] | None = None
     contacts: list[ContactSyncModel] | None = None
     creditMemoApplications: list[CreditMemoAppliedSyncModel] | None = None
     invoices: list[InvoiceSyncModel] | None = None
     invoiceLines: list[InvoiceLineSyncModel] | None = None
     customFields: list[CustomFieldSyncModel] | None = None
     payments: list[PaymentSyncModel] | None = None
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/bulkcurrencyconversionmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/bulkcurrencyconversionmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/bulkdeleterequestmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/bulkdeleterequestmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/cashflowreportmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/cashflowreportmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/codedefinitionmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/codedefinitionmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/companydetailsmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/companydetailsmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/companydetailspaymentmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/companydetailspaymentmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/companymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/companymodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,16 @@
     publicUrlSlug: str | None = None
     stateTaxId: str | None = None
     stateOfIncorporation: str | None = None
     linkedInUrlSlug: str | None = None
     isVerified: bool | None = None
     lastVerifiedDate: str | None = None
     viewBoxSettings: ViewBoxSettingsModel | None = None
+    serviceFabricOrgId: str | None = None
+    serviceFabricCompanyId: str | None = None
     notes: list[NoteModel] | None = None
     attachments: list[AttachmentModel] | None = None
     contacts: list[ContactModel] | None = None
     invoices: list[object] | None = None
     customFieldDefinitions: list[CustomFieldDefinitionModel] | None = None
     customFieldValues: list[CustomFieldValueModel] | None = None
     companyClassificationCodeDefinition: CodeDefinitionModel | None = None
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/companysyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/companysyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/connectorinfomodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/connectorinfomodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/contactmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/contactmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/contactsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/contactsyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/countrymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/countrymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/creditmemoappliedmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/creditmemoappliedmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/creditmemoappliedsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/creditmemoappliedsyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/creditmemoinvoicemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/creditmemoinvoicemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/currencymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/currencymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/currencyratemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/currencyratemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/customersummarymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/customersummarymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/customfielddefinitionmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/customfielddefinitionmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/customfieldsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/customfieldsyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/customfieldvaluemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/customfieldvaluemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/dailypayableoutstandingreportmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/dailypayableoutstandingreportmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/dailysalesoutstandingreportmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/dailysalesoutstandingreportmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/deleteresult.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/deleteresult.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/developeraccountsubmitmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/developeraccountsubmitmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/dposummarygrouptotalmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/dposummarygrouptotalmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/dposummarymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/dposummarymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/erpmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/erpmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/errorresult.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/errorresult.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/featureflagsrequestmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/featureflagsrequestmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/featureflagsresponsemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/featureflagsresponsemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountbalancehistorymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountbalancehistorymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountbalancehistorysyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountbalancehistorysyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialaccountsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialaccountsyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialreportcellmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialreportcellmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialreportmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialreportmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialreportrowmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialreportrowmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialyearsettingmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialyearsettingmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/financialyearsettingsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/financialyearsettingsyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/groupaccountmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/groupaccountmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invitedatamodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invitedatamodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invitemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invitemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invitesubmitmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invitesubmitmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoiceaddressmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoiceaddressmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicehistorymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicehistorymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicelinemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicelinemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicelinesyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicelinesyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicepaymentdetailmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicepaymentdetailmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicesummarymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicesummarymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicesummarymodelinvoicesummarytotalsmodelsummaryfetchresult.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicesummarymodelinvoicesummarytotalsmodelsummaryfetchresult.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicesummarytotalsmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicesummarytotalsmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/invoicesyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/invoicesyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/leadmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/leadmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/magiclinkmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/magiclinkmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/magiclinkstatusmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/magiclinkstatusmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/notemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/notemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/payablescomingdueheadermodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/payablescomingdueheadermodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/payablescomingduemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/payablescomingduemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/payablescomingduewidgetmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/payablescomingduewidgetmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/payablessummaryreportmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/payablessummaryreportmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentappliedmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentappliedmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentappliedsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentappliedsyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentdetailheadermodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentdetailheadermodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentdetailmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentdetailmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,13 +55,14 @@
     modifiedUserId: str | None = None
     appEnrollmentId: str | None = None
     isVoided: bool | None = None
     inDispute: bool | None = None
     currencyRate: float | None = None
     baseCurrencyPaymentAmount: float | None = None
     baseCurrencyUnappliedAmount: float | None = None
+    serviceFabricStatus: str | None = None
     applications: list[PaymentAppliedModel] | None = None
     notes: list[NoteModel] | None = None
     attachments: list[AttachmentModel] | None = None
     customFieldDefinitions: list[CustomFieldDefinitionModel] | None = None
     customFieldValues: list[CustomFieldValueModel] | None = None
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentsummarymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentsummarymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentsummarymodelpaymentsummarytotalsmodelsummaryfetchresult.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentsummarymodelpaymentsummarytotalsmodelsummaryfetchresult.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentsummarytotalsmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentsummarytotalsmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/paymentsyncmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/paymentsyncmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/publiccompanyprofilemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/publiccompanyprofilemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/riskratemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/riskratemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/statemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/statemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/statusmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/statusmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/summaryagingtotalsmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/summaryagingtotalsmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/supportaccessmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/supportaccessmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/supportaccessrequest.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/supportaccessrequest.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/syncentityresultmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/syncentityresultmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/syncrequestmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/syncrequestmodel.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,14 @@
     syncRequestId: str | None = None
     groupKey: str | None = None
     statusCode: str | None = None
     operationTypeName: str | None = None
     operationType: int | None = None
     processResultMessage: str | None = None
     failureCount: int | None = None
-    runFullSync: str | None = None
+    runFullSync: bool | None = None
     appEnrollmentId: str | None = None
     created: str | None = None
     modified: str | None = None
     modifiedUserId: str | None = None
     details: object | None = None
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/syncsubmitmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/syncsubmitmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transactiondetailmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transactiondetailmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transactionmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transactionmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transactionmodeltransactionsummarytotalmodelsummaryfetchresult.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transactionmodeltransactionsummarytotalmodelsummaryfetchresult.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 from lockstep.models.transactionmodel import TransactionModel
 from lockstep.models.transactionsummarytotalmodel import TransactionSummaryTotalModel
 from lockstep.models.summaryagingtotalsmodel import SummaryAgingTotalsModel
 
 @dataclass
 class TransactionModelTransactionSummaryTotalModelSummaryFetchResult:
 
-    records: list[TransactionModel] | None = None
     totalCount: int | None = None
     pageSize: int | None = None
     pageNumber: int | None = None
+    records: list[TransactionModel] | None = None
     summary: TransactionSummaryTotalModel | None = None
     agingSummary: list[SummaryAgingTotalsModel] | None = None
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transactionsummarytotalmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transactionsummarytotalmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transcriptionrequestsubmit.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transcriptionrequestsubmit.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transcriptionvalidationrequestitemmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transcriptionvalidationrequestitemmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transcriptionvalidationrequestmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transcriptionvalidationrequestmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transferownermodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transferownermodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/transferownersubmitmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/transferownersubmitmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/urimodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/urimodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/useraccountmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/useraccountmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/userdataresponsemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/userdataresponsemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/usergroupmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/usergroupmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/userrolemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/userrolemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/vendorsummarymodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/vendorsummarymodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/viewboxsettingsmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/viewboxsettingsmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/webhookhistorytablestoragemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/webhookhistorytablestoragemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/webhookmodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/webhookmodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep/models/webhookrulemodel.py` & `lockstep-sdk-2023.7.7/src/lockstep/models/webhookrulemodel.py`

 * *Files identical despite different names*

### Comparing `lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/PKG-INFO` & `lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockstep-sdk
-Version: 2023.5.21
+Version: 2023.7.7
 Summary: Lockstep Platform SDK for Python
 Home-page: https://github.com/Lockstep-Network/lockstep-sdk-python
 Author: Lockstep
 Author-email: developer@lockstep.io
 Project-URL: Bug Tracker, https://github.com/Lockstep-Network/lockstep-sdk-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lockstep-sdk-2023.5.21/src/lockstep_sdk.egg-info/SOURCES.txt` & `lockstep-sdk-2023.7.7/src/lockstep_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

