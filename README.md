# ![LOGO](logo.png) Adyen Payout Service MSP Connector

## Description

A generated MSP connector for the Adyen Payout Service API (version 30).

Generated from: https://api.apis.guru/v2/specs/adyen.com/PayoutService/30/openapi.json<br/>
Generated at: 2019-05-07T11:15:13+03:00

## API Description

A set of API endpoints that allow you to store payout details, confirm, or decline a payout.

For more information, refer to [Third-party payouts](https://docs.adyen.com/developers/features/third-party-payouts).

## Authorization

This API does not require authorization.

## Actions

### Confirms a payout.

> Confirms a previously submitted payout.<br/>
> <br/>
> To cancel a payout, use the `/declineThirdParty` endpoint.

### Cancels a payout.

> Cancels a previously submitted payout.<br/>
> <br/>
> To confirm and send a payout, use the `/confirmThirdParty` endpoint.

### Pay out directly.

> With this call, you can pay out to your customers, and funds will be made available within 30 minutes on the cardholder's bank account (this is dependent on whether the issuer supports this functionality). Instant card payouts are only supported for Visa and Mastercard cards.

### Stores payout details.

> Stores payment details under the `PAYOUT` recurring contract. These payment details can be used later to submit a payout via the `/submitThirdParty` call.

### Stores details and submits a payout.

> Submits a payout and stores its details for subsequent payouts.<br/>
> <br/>
> The submitted payout must be confirmed or declined either by a reviewer or via `/confirmThirdParty` or `/declineThirdParty` calls.

### Submits a payout.

> Submits a payout using the previously stored payment details. To store payment details, use the `/storeDetail` API call.<br/>
> <br/>
> The submitted payout must be confirmed or declined either by a reviewer or via `/confirmThirdParty` or `/declineThirdParty` calls.

## License

flowground :- Telekom iPaaS / adyen-com-payout-service-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
