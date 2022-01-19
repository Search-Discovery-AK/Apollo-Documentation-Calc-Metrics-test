# Wishlist Shared

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];;;
appEventData.push({
  "event": "Wishlist Shared",
    "product": [
        {
            "price": {
                "priceType": "<priceType>",
                "sellingPrice": "<sellingPrice>"
            },
            "productInfo": {
                "productID": "<productID>",
                "sku": "<sku>"
            }
        }
    ],
    "wishlist": {
        "total": {
            "currency": "<currency>",
            "value": "<value>"
        },
        "wishlistID": "<wishlistID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|currency|string|Currency of the transaction. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|priceType|string|Describes the type of price offered using commonly used terms. |1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|sku|string|Stock Keeping Unit \(SKU\) Unique Identifier of specific item \(typically\) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|value|string|String representation of the total value of all products in a wishlist. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22|^[0-9]*(\.[0-9]{1,2})?$||||||
|wishlistID|string|Back-end identifier for a wishlist|12345, 435678, 34567, XCV456, XCV876|||||||




