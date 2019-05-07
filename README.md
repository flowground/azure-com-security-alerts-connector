# ![LOGO](logo.png) Security Center **flow**ground Connector

## Description

A generated **flow**ground connector for the Security Center API (version 2019-01-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/security-alerts/2019-01-01/swagger.json<br/>
Generated at: 2019-05-07T17:38:49+03:00

## API Description

API spec for Microsoft.Security (Azure Security Center) resource provider

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### List all the alerts that are associated with the subscription

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `$filter` - _optional_ - OData filter. Optional.
* `$select` - _optional_ - OData select. Optional.
* `$expand` - _optional_ - OData expand. Optional.

### List all the alerts that are associated with the subscription that are stored in a specific location

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `ascLocation` - _required_ - The location where ASC stores the data of the subscription. can be retrieved from Get locations
* `$filter` - _optional_ - OData filter. Optional.
* `$select` - _optional_ - OData select. Optional.
* `$expand` - _optional_ - OData expand. Optional.

### Get an alert that is associated with a subscription

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `ascLocation` - _required_ - The location where ASC stores the data of the subscription. can be retrieved from Get locations
* `alertName` - _required_ - Name of the alert object

### Update the alert's state

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `ascLocation` - _required_ - The location where ASC stores the data of the subscription. can be retrieved from Get locations
* `alertName` - _required_ - Name of the alert object
* `alertUpdateActionType` - _required_ - Type of the action to do on the alert
    Possible values: Dismiss, Reactivate.

### List all the alerts that are associated with the resource group

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `$filter` - _optional_ - OData filter. Optional.
* `$select` - _optional_ - OData select. Optional.
* `$expand` - _optional_ - OData expand. Optional.

### List all the alerts that are associated with the resource group that are stored in a specific location

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `ascLocation` - _required_ - The location where ASC stores the data of the subscription. can be retrieved from Get locations
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.
* `$filter` - _optional_ - OData filter. Optional.
* `$select` - _optional_ - OData select. Optional.
* `$expand` - _optional_ - OData expand. Optional.

### Get an alert that is associated a resource group or a resource in a resource group

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `ascLocation` - _required_ - The location where ASC stores the data of the subscription. can be retrieved from Get locations
* `alertName` - _required_ - Name of the alert object
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.

### Update the alert's state

*Tags:* `Alerts`

#### Input Parameters
* `api-version` - _required_ - API version for the operation
* `subscriptionId` - _required_ - Azure subscription ID
* `ascLocation` - _required_ - The location where ASC stores the data of the subscription. can be retrieved from Get locations
* `alertName` - _required_ - Name of the alert object
* `alertUpdateActionType` - _required_ - Type of the action to do on the alert
    Possible values: Dismiss, Reactivate.
* `resourceGroupName` - _required_ - The name of the resource group within the user's subscription. The name is case insensitive.

## License

**flow**ground :- Telekom iPaaS / azure-com-security-alerts-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
