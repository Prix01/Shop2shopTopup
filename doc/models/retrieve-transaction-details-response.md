
# Retrieve Transaction Details Response

## Structure

`RetrieveTransactionDetailsResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `reference` | `?string` | Optional | The reference for the transaction | getReference(): ?string | setReference(?string reference): void |
| `prixAccount` | `?string` | Optional | The Prix account associated with the transaction | getPrixAccount(): ?string | setPrixAccount(?string prixAccount): void |
| `externalID` | `?string` | Optional | The external ID associated with the transaction | getExternalID(): ?string | setExternalID(?string externalID): void |
| `amount` | `?float` | Optional | The amount of the transaction | getAmount(): ?float | setAmount(?float amount): void |

## Example (as JSON)

```json
{
  "reference": null,
  "prixAccount": null,
  "externalID": null,
  "amount": null
}
```

