---
slug: /poscreators/get-started/checklist
title: Integration Checklist
---

# Integration Checklist
Integrating the Middleware involves several steps, from calling the API the right way to registering in the production Portal and connecting to Dealers. To simplify this process for POS Creators, we've composed a concise checklist that can be used to validate if all required steps were succesfully performed.

| Country | Check | Description | Docs |
| :----: | ----- | ----------- | --------- |
| ![All markets](images/flag-eu.png) | **Sandbox Portal account created** | An account in the sandbox Portal was created to create test Middleware instances | [Getting Started Guide](README.md) |
| ![All markets](images/flag-eu.png) | **API methods are implemented** | The POS System can call the Middleware's API via the protocol of choice | [Function structures](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/general/function-structures) & <br /> [Communication protocols](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/general/communication) |
| ![All markets](images/flag-eu.png) | **Business sequences are implemented** | The required business cases (i.e. the `ftReceiptCases`, `ftChargeItemCases` and `ftPayItemCases`) are implemented. Depending on the POS system, not all cases might be required (only those which make sense for your use case). | [Receipt cases](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/general/reference-tables) & relevant country-specific appendices |
| ![All markets](images/flag-eu.png) | **Receipt headers are included** | The correct values are passed for `ftCashBoxID`, `ftPosSystemID`, `cbTerminalID`, `cbReceiptReference` and `cbReceiptMoment`. | [Data structures](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/general/data-structures) & relevant country-specific appendices |
| ![All markets](images/flag-eu.png) | **Closing receipts are implemented** | Daily, monthly and yearly closing receipts are implemented via the respective ´ftRecreiptCases`. | [Receipt cases](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/general/reference-tables) & relevant country-specific appendices |
| ![All markets](images/flag-eu.png) | **Error handling is implemented** | The different types of errors (Middleware not reachable & signing device/service not reachable) are properly handled by the POS software | [Cash register integration](https://docs.fiskaltrust.cloud/docs/poscreators/middleware-doc/general/cash-register-integration) & relevant country-specific appendices |
| ![All markets](images/flag-eu.png) | **Production Portal account created** | An account in the production Portal was created to manage POS Systems. | [Getting Started Guide](README.md) |
| ![All markets](images/flag-eu.png) | **POS Systems are created in the production Portal** | One POS System per model (not per actual device) is created in the Portal, and its ID is used as `cbPosSystemID` in sign requests. | [Getting Started Guide](README.md) |
| ![All markets](images/flag-eu.png) | **POS Dealers are invited and connected to POS Systems** | The POS Dealers distributing the device are either invited by their POS Creator or created their accounts themselves, and are connected to the previously created POS System. | [Getting Started Guide](README.md) |
