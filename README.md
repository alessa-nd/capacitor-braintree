# WORK IN PROGRESS

Android still not implemented.

# @moovenda/capacitor-braintree

Capacitor v3+ Braintree Native SDK plugin

## Install

```bash
npm install @moovenda/capacitor-braintree
npx cap sync
```

## API

<docgen-index>

* [`setToken(...)`](#settoken)
* [`showDropIn(...)`](#showdropin)
* [`getDeviceData(...)`](#getdevicedata)
* [Interfaces](#interfaces)

</docgen-index>

<docgen-api>
<!--Update the source file JSDoc comments and rerun docgen to update the docs below-->

### setToken(...)

```typescript
setToken(options: DropInToken) => any
```

| Param         | Type                                                |
| ------------- | --------------------------------------------------- |
| **`options`** | <code><a href="#dropintoken">DropInToken</a></code> |

**Returns:** <code>any</code>

--------------------


### showDropIn(...)

```typescript
showDropIn(options: DropInOptions) => any
```

| Param         | Type                                                    |
| ------------- | ------------------------------------------------------- |
| **`options`** | <code><a href="#dropinoptions">DropInOptions</a></code> |

**Returns:** <code>any</code>

--------------------


### getDeviceData(...)

```typescript
getDeviceData(options: DataCollectorOptions) => any
```

| Param         | Type                                                                  |
| ------------- | --------------------------------------------------------------------- |
| **`options`** | <code><a href="#datacollectoroptions">DataCollectorOptions</a></code> |

**Returns:** <code>any</code>

--------------------


### Interfaces


#### DropInToken

| Prop        | Type                |
| ----------- | ------------------- |
| **`token`** | <code>string</code> |


#### DropInOptions

| Prop                    | Type                |
| ----------------------- | ------------------- |
| **`amount`**            | <code>string</code> |
| **`disabled`**          | <code>{}</code>     |
| **`givenName`**         | <code>string</code> |
| **`surname`**           | <code>string</code> |
| **`email`**             | <code>string</code> |
| **`phoneNumber`**       | <code>string</code> |
| **`streetAddress`**     | <code>string</code> |
| **`postalCode`**        | <code>string</code> |
| **`locality`**          | <code>string</code> |
| **`countryCodeAlpha2`** | <code>string</code> |


#### DropInResult

| Prop                       | Type                                                                                                                                                                            |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`cancelled`**            | <code>boolean</code>                                                                                                                                                            |
| **`nonce`**                | <code>string</code>                                                                                                                                                             |
| **`type`**                 | <code>string</code>                                                                                                                                                             |
| **`localizedDescription`** | <code>string</code>                                                                                                                                                             |
| **`deviceData`**           | <code>string</code>                                                                                                                                                             |
| **`card`**                 | <code>{ lastTwo: string; network: string; }</code>                                                                                                                              |
| **`payPalAccount`**        | <code>{ email: string; firstName: string; lastName: string; phone: string; billingAddress: string; shippingAddress: string; clientMetadataId: string; payerId: string; }</code> |
| **`applePaycard`**         | <code>any</code>                                                                                                                                                                |
| **`threeDSecureCard`**     | <code>{ liabilityShifted: boolean; liabilityShiftPossible: boolean; }</code>                                                                                                    |
| **`venmoAccount`**         | <code>{ username: string; }</code>                                                                                                                                              |


#### DataCollectorOptions

| Prop             | Type                |
| ---------------- | ------------------- |
| **`merchantId`** | <code>string</code> |

</docgen-api>
