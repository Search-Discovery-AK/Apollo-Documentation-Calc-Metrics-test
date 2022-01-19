# Listing Sort Order Changed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];;;
appEventData.push({
  "event": "Listing Sort Order Changed",
    "listingRefined": {
        "filterList": "<filterList>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|filterList|string|A twice delimited string of filterType and filterValue pairs.  Use \~ between type and value.  Use \| between pairs|sort\~price ascending\|color\~green\|size\~medium|||||||




