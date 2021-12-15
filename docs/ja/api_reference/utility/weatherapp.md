# WeatherApp


天気連携に関する機能を提供するutility

## Table of contents

### Methods

- [getCityCode](weatherapp.md#getcitycode)
- [getCityWeather](weatherapp.md#getcityweather)
- [getPrefCode](weatherapp.md#getprefcode)
- [getPrefWeather](weatherapp.md#getprefweather)
- [getWeatherByName](weatherapp.md#getweatherbyname)

## Methods

### getCityCode

▸ **getCityCode**(`name`: *string*, `prefCode`: *string*): [*City*](city.md)[]

指定された名前に前方一致する市区町村コードを取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | 取得する市区町村名（前方一致） |
| `prefCode` | *string* | - |

**Returns:** [*City*](city.md)[]

___

### getCityWeather

▸ **getCityWeather**(`code`: *string* \| *number*): ``null`` \| [*ForecastResult*](forecastresult.md)

指定された市区町村コードで本日の天気予報を取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `code` | *string* \| *number* | 市区町村コード |

**Returns:** ``null`` \| [*ForecastResult*](forecastresult.md)

▸ **getCityWeather**(`code`: *string* \| *number*, `day`: *string*): ``null`` \| [*ForecastResult*](forecastresult.md)

指定された市区町村コードと日でで天気予報を取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `code` | *string* \| *number* | 市区町村コード |
| `day` | *string* | 日(TODAY or TOMORROW or TODAY_AND_TOMORROW) |

**Returns:** ``null`` \| [*ForecastResult*](forecastresult.md)

___

### getPrefCode

▸ **getPrefCode**(`name`: *string*): [*Pref*](pref.md)[]

指定された名前に前方一致する県コードを取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | 取得する県名（前方一致） |

**Returns:** [*Pref*](pref.md)[]

___

### getPrefWeather

▸ **getPrefWeather**(`code`: *string*): ``null`` \| [*ForecastResult*](forecastresult.md)

指定された県コードで本日の天気予報を取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `code` | *string* | 県コード |

**Returns:** ``null`` \| [*ForecastResult*](forecastresult.md)

▸ **getPrefWeather**(`code`: *string*, `day`: *string*): ``null`` \| [*ForecastResult*](forecastresult.md)

指定された県コードと日で天気予報を取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `code` | *string* | 県コード |
| `day` | *string* | 日（TODAY or TOMORROW or TODAY_AND_TOMORROW） |

**Returns:** ``null`` \| [*ForecastResult*](forecastresult.md)

___

### getWeatherByName

▸ **getWeatherByName**(`name`: *string*): [*ForecastResult*](forecastresult.md)[]

指定された名前に前方一致する地域の本日の天気予報のリストを取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | 天気を取得する地名 ("神奈川県", "神奈川県 川崎市", "神奈川県 川崎市 多摩区"などスペース区切りで入力してください) |

**Returns:** [*ForecastResult*](forecastresult.md)[]

▸ **getWeatherByName**(`name`: *string*, `day`: *string*): [*ForecastResult*](forecastresult.md)[]

指定された名前に前方一致する地域の指定した日の天気予報のリスト取得します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | 天気を取得する地名 ("神奈川県", "神奈川県 川崎市", "神奈川県 川崎市 多摩区"などスペース区切りで入力してください) |
| `day` | *string* | 日(TODAY or TOMORROW or TODAY_AND_TOMORROW) |

**Returns:** [*ForecastResult*](forecastresult.md)[]
