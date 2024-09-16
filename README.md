# UsenetCompass.github.io

## Json Data

```Json
{
    "Offer": "An offer",
    "Provider": "The Provider",
    "Type": "Subscription",
    "Retention": 200,
    "Speed": "Unlimited",
    "Connections": 10,
    "Size": "Unlimited",
    "Price": 5,
    "Currency": "USD",
    "Backbone": "The Best",
    "Deals": false,
    "Remarks": "Any remark",
    "URL": "http://localhost/"
}
```

### Field Descriptions

- Offer: (Optional) A string representing the name of the offer. Its value is not displayed and is not mandatory.

- Provider: A string that corresponds to the first column of the associated table, indicating the service provider.

- Type: A string that must be either "Subscription" or "Block", indicating the type of service offered.

- Retention: A mandatory integer representing the retention period in days.

- Speed: A string that can specify the maximum speed in Mbit, or can be "Variable" or "Unlimited".

- Connections: An integer indicating the maximum number of simultaneous connections allowed.

- Size (GB): A string representing the size in gigabytes (GB). For "Block" type offers, this indicates the total size.

- Price: A string without the currency. For subscription types, this should represent the monthly price, calculated as the annual price divided by 12.

- Currency: A string value that represents the price currency.

- Backbone: A string that indicates the backbone provider, which is specified in parentheses in the first column of the table. This value can be filtered using the select option in the footer of the table.

- Deals: A boolean value. If the offer is listed in `normal.json`, this should be false. If it is in `deals.json`, it should be true.

- Remarks: A string for any additional comments or notes regarding the offer.

- URL: A string that can either be the URL of the offer or the URL of the provider.

## How to help me

- I convert JSON to CSV and modify it using LibreOffice Calc
- Sometimes I need to change `"Deals":"FALSE"` -> `"Deals":false`
- Create a PR :)

## Sources

- For the retention and the backbones: https://www.reddit.com/r/usenet/comments/lwupx3/updated_usenet_provider_map/
- For the deals: https://www.reddit.com/r/usenet/wiki/providerdeals/
