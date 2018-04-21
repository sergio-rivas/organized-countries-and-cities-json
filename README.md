# Open City Database

The idea is to make a series of JSON files that all follow the same format to easily integrate with web projects.

## Format

For all files, please save as the country name in parameterized notation.
Ex:  st-kitts-and-neves.json, united-states-of-america.json, china.json

## JSON Structure

For each "country file", please try to add english & the local language. If you can add other languages, that would be helpful too.
The idea is that the database of json files should become increasingly more complete.
If a country does not have provinces, please write "has_provinces": false, then include its city list in the same format.

Example of Structure:

```
{
  "country_name_en": "China",
  "country_name_zh": "中国",
  "has_provinces": true,
  "provinces": [
    {
      "province_name_en": "Zhejiang",
      "province_name_zh": "浙江省",
      "cities": [
        {
          "city_name_en": "Hangzhou",
          "city_name_zh": "杭州市",
          "prefecture": "Hangzhou"
        },
        {},
        {},
        etc.
      ]
    },
    {},
    {},
    etc.
  ]
 }
```
## Completed Countries

- China
