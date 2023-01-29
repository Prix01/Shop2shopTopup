# API

```php
$aPIController = $client->getAPIController();
```

## Class Name

`APIController`

## Methods

* [Retrieve Transaction Details](../../doc/controllers/api.md#retrieve-transaction-details)
* [Create a New Transaction](../../doc/controllers/api.md#create-a-new-transaction)


# Retrieve Transaction Details

Retrieves transaction details for the specified external ID.

```php
function retrieveTransactionDetails(string $externalID): RetrieveTransactionDetailsResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `externalID` | `string` | Template, Required | The external ID associated with the transaction |

## Response Type

[`RetrieveTransactionDetailsResponse`](../../doc/models/retrieve-transaction-details-response.md)

## Example Usage

```php
$externalID = 'externalID8';

$result = $aPIController->retrieveTransactionDetails($externalID);
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Invalid request | `ApiException` |


# Create a New Transaction

Creates a new transaction with the specified details

```php
function createANewTransaction(string $externalID, string $reference, string $prixAccount, float $amount): void
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `externalID` | `string` | Template, Required | The external ID associated with the transaction |
| `reference` | `string` | Query, Required | The reference for the transaction |
| `prixAccount` | `string` | Query, Required | The Prix account associated with the transaction |
| `amount` | `float` | Query, Required | The amount of the transaction |

## Response Type

`void`

## Example Usage

```php
$externalID = 'externalID8';
$reference = 'reference4';
$prixAccount = 'prixAccount2';
$amount = 56.78;

$aPIController->createANewTransaction($externalID, $reference, $prixAccount, $amount);
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Invalid request | `ApiException` |

