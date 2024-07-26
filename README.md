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
    "Backbone": "The Best",
    "Deals": false,
    "Remarks": "Any remark",
    "URL": "http://localhost/"
  }
```
In the JSON object above:
- "Offer" is a string, its value is not show, it's not mandatory
- "Provider" is a string, its value is the first column of the table
- "Type" should have one of the two values: "Subscription"/"Block"
- "Retention" is a mandatory number, in days
- "Speed" is a string, it can contain the max speed in Mbit, or "Variable" or "Unlimited"
- "Connections": 40,
- "Size (GB)" is a string, in GB, in case of a Block it is its size
- "Price" is a string, that contains its currency. In case it's a subscription, it's the annual price divided per 12
- "Backbone" is a string, its value is in parenthesis in the first column of the table and it can be filtered by the select in the footer of the table
- "Deals" is a boolean, if it's in the `normal.json`, should be false, else in the `deals.json` true
- "Remarks" is a string
- "URL" is a string, it can be the url of the offer or the url of the provider

## How to help me

- I convert JSON to CSV and modify it using LibreOffice Calc
- Sometimes I need to change `"Deals":"FALSE"` -> `"Deals":false`
- Create a PR :)

## Sources

- For the retention and the backbones: https://www.reddit.com/r/usenet/comments/lwupx3/updated_usenet_provider_map/
- For the deals: https://www.reddit.com/r/usenet/wiki/providerdeals/
