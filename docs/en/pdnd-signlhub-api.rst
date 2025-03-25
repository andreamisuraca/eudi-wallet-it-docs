.. include:: ../common/common_definitions.rst

.. role:: raw-html(raw)
   :format: html

PDND SignalHub API
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Authentic Sources
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Authentic Sources MUST perform the following actions through PDND:

    - enable the SignalHub feature for each credential e-service via GUI
    - submit a signal for each e-service output data variation

.. note::
    A complete OpenAPI Specification is available :raw-html:`<a href="https://github.com/pagopa/interop-signalhub-core/blob/main/docs/openAPI/push-signals.yaml" target="_blank">here</a>`.


Credential Issuer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Credential Issuers MUST perform the following actions through PDND:

    - monitor data changes for each e-service with SignalHub enabled
    - retrieve the updated data from the subscribed e-service

.. note::
    A complete OpenAPI Specification is available :raw-html:`<a href="https://github.com/pagopa/interop-signalhub-core/blob/main/docs/openAPI/pull-signals.yaml" target="_blank">here</a>`.


Notify Update Credential
...........................................

.. list-table::
    :widths: 20 80 
    :stub-columns: 1

    * - **Description**
      - The service is designed to allow Authentic Source (AS), via SignalHub, to submit
        notification of a change of status and/or value of a specific attribute (e.g. MDL)
        associated with a digital document issued by the Credential Issuer.
    * - **Provider**
      - PDND
    * - **Consumer**
      - Authentic Source


Check for Update Credential
...........................................

.. list-table::
    :widths: 20 80 
    :stub-columns: 1

    * - **Description**
      - The service is designed to allow Credential Issuers (CI), via SignalHub, to check
        for changes in the status and/or value of a specific attribute (e.g. MDL)
        as notified by the Authentic Source. The CI
    * - **Provider**
      - PDND
    * - **Consumer**
      - Credential Issuers
