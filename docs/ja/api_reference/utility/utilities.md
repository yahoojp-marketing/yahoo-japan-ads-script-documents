# Utilities


様々な操作を提供するUtilityです。

## Table of contents

### Methods

- [formatDate](utilities.md#formatdate)
- [sleep](utilities.md#sleep)

## Methods

### formatDate

▸ **formatDate**(`date`: Date, `timeZone`: *string*, `format`: *string*): *string*

指定された日付を文字列にフォーマット

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `date` | Date | 文字列としてフォーマットする日付 |
| `timeZone` | *string* | 結果の出力タイムゾーン |
| `format` | *string* | 下表に従ったフォーマット<br> 例は 2021-07-09T13:07:04.054 Asia/Tokyo<br> <p>&nbsp;</p> <figure> <table> <thead> <tr><th>Standalone token</th><th>Format token</th><th>Description</th><th>Example</th></tr> </thead> <tbody> <tr><td>S</td><td>&nbsp;</td><td>millisecond, no padding</td><td><code>54</code></td></tr> <tr><td>SSS</td><td>&nbsp;</td><td>millisecond, padded to 3</td><td><code>054</code></td></tr> <tr><td>u</td><td>&nbsp;</td><td>fractional seconds, functionally identical to SSS</td><td><code>054</code></td></tr> <tr><td>s</td><td>&nbsp;</td><td>second, no padding</td><td><code>4</code></td></tr> <tr><td>ss</td><td>&nbsp;</td><td>second, padded to 2 padding</td><td><code>04</code></td></tr> <tr><td>m</td><td>&nbsp;</td><td>minute, no padding</td><td><code>7</code></td></tr> <tr><td>mm</td><td>&nbsp;</td><td>minute, padded to 2</td><td><code>07</code></td></tr> <tr><td>h</td><td>&nbsp;</td><td>hour in 12-hour time, no padding</td><td><code>1</code></td></tr> <tr><td>hh</td><td>&nbsp;</td><td>hour in 12-hour time, padded to 2</td><td><code>01</code></td></tr> <tr><td>H</td><td>&nbsp;</td><td>hour in 24-hour time, no padding</td><td><code>13</code></td></tr> <tr><td>HH</td><td>&nbsp;</td><td>hour in 24-hour time, padded to 2</td><td><code>13</code></td></tr> <tr><td>Z</td><td>&nbsp;</td><td>narrow offset</td><td><code>+9</code></td></tr> <tr><td>ZZ</td><td>&nbsp;</td><td>short offset</td><td><code>+09:00</code></td></tr> <tr><td>ZZZ</td><td>&nbsp;</td><td>techie offset</td><td><code>+0900</code></td></tr> <tr><td>ZZZZ</td><td>&nbsp;</td><td>abbreviated named offset</td><td><code>GTM+9</code></td></tr> <tr><td>ZZZZZ</td><td>&nbsp;</td><td>unabbreviated named offset</td><td><code>Japan Standard Time</code></td></tr> <tr><td>z</td><td>&nbsp;</td><td>IANA zone</td><td><code>Asia/Tokyo</code></td></tr> <tr><td>a</td><td>&nbsp;</td><td>meridiem</td><td><code>AM</code></td></tr> <tr><td>d</td><td>&nbsp;</td><td>day of the month, no padding</td><td><code>9</code></td></tr> <tr><td>dd</td><td>&nbsp;</td><td>day of the month, padded to 2</td><td><code>09</code></td></tr> <tr><td>c</td><td>E</td><td>day of the week, as number from 1-7 (Monday is 1, Sunday is 7)</td><td><code>5</code></td></tr> <tr><td>ccc</td><td>EEE</td><td>day of the week, as an abbreviate localized string</td><td><code>Fri</code></td></tr> <tr><td>cccc</td><td>EEEE</td><td>day of the week, as an unabbreviated localized string</td><td><code>Friday</code></td></tr> <tr><td>ccccc</td><td>EEEEE</td><td>day of the week, as a single localized letter</td><td><code>F</code></td></tr> <tr><td>L</td><td>M</td><td>month as an unpadded number</td><td><code>7</code></td></tr> <tr><td>LL</td><td>MM</td><td>month as an padded number</td><td><code>07</code></td></tr> <tr><td>LLL</td><td>MMM</td><td>month as an abbreviated localized string</td><td><code>Jul</code></td></tr> <tr><td>LLLL</td><td>MMMM</td><td>month as an unabbreviated localized string</td><td><code>July</code></td></tr> <tr><td>LLLLL</td><td>MMMMM</td><td>month as a single localized letter</td><td><code>J</code></td></tr> <tr><td>y</td><td>&nbsp;</td><td>year, unpadded</td><td><code>2021</code></td></tr> <tr><td>yy</td><td>&nbsp;</td><td>two-digit year</td><td><code>21</code></td></tr> <tr><td>yyyy</td><td>&nbsp;</td><td>four- to six- digit year, pads to 4</td><td><code>2021</code></td></tr> <tr><td>G</td><td>&nbsp;</td><td>abbreviated localized era</td><td><code>AD</code></td></tr> <tr><td>GG</td><td>&nbsp;</td><td>unabbreviated localized era</td><td><code>Anno Domini</code></td></tr> <tr><td>GGGGG</td><td>&nbsp;</td><td>one-letter localized era</td><td><code>A</code></td></tr> <tr><td>kk</td><td>&nbsp;</td><td>ISO week year, unpadded</td><td><code>21</code></td></tr> <tr><td>kkkk</td><td>&nbsp;</td><td>ISO week year, padded to 4</td><td><code>2021</code></td></tr> <tr><td>W</td><td>&nbsp;</td><td>ISO week number, unpadded</td><td><code>27</code></td></tr> <tr><td>WW</td><td>&nbsp;</td><td>ISO week number, padded to 2</td><td><code>27</code></td></tr> <tr><td>o</td><td>&nbsp;</td><td>ordinal (day of year), unpadded</td><td><code>190</code></td></tr> <tr><td>ooo</td><td>&nbsp;</td><td>ordinal (day of year), padded to 3</td><td><code>190</code></td></tr> <tr><td>q</td><td>&nbsp;</td><td>quarter, no padding</td><td><code>3</code></td></tr> <tr><td>qq</td><td>&nbsp;</td><td>quarter, padded to 2</td><td><code>03</code></td></tr> <tr><td>D</td><td>&nbsp;</td><td>localized numeric date</td><td><code>2021/7/9</code></td></tr> <tr><td>DD</td><td>&nbsp;</td><td>localized date with abbreviated month</td><td><code>2021年7月9日</code></td></tr> <tr><td>DDD</td><td>&nbsp;</td><td>localized date with full month</td><td><code>2021年7月9日</code></td></tr> <tr><td>DDDD</td><td>&nbsp;</td><td>localized date with full month and weekday</td><td><code>2021年7月9日金曜日</code></td></tr> <tr><td>t</td><td>&nbsp;</td><td>localized time</td><td><code>13:07</code></td></tr> <tr><td>tt</td><td>&nbsp;</td><td>localized time with seconds</td><td><code>13:07:04</code></td></tr> <tr><td>ttt</td><td>&nbsp;</td><td>localized time with seconds and abbreviated offset</td><td><code>13:07:04 JST</code></td></tr> <tr><td>tttt</td><td>&nbsp;</td><td>localized time with seconds and full offset</td><td><code>13時07分04秒 日本標準時</code></td></tr> <tr><td>T</td><td>&nbsp;</td><td>localized 24-hour time</td><td><code>13:07</code></td></tr> <tr><td>TT</td><td>&nbsp;</td><td>localized 24-hour time with seconds</td><td><code>13:07:04</code></td></tr> <tr><td>TTT</td><td>&nbsp;</td><td>localized 24-hour time with seconds and abbreviated offset</td><td><code>13:07:04 JST</code></td></tr> <tr><td>TTTT</td><td>&nbsp;</td><td>localized 24-hour time with seconds and full offset</td><td><code>13:07:04 日本標準時</code></td></tr> <tr><td>f</td><td>&nbsp;</td><td>short localized date and time</td><td><code>2021/7/9 13:07</code></td></tr> <tr><td>ff</td><td>&nbsp;</td><td>less short localized date and time</td><td><code>2021年7月9日 13:07</code></td></tr> <tr><td>fff</td><td>&nbsp;</td><td>verbose localized date and time</td><td><code>2021年7月9日 13:07 JST</code></td></tr> <tr><td>ffff</td><td>&nbsp;</td><td>extra verbose localized date and time</td><td><code>2021年7月9日金曜日 13:07 日本標準時</code></td></tr> <tr><td>F</td><td>&nbsp;</td><td>short localized date and time with seconds</td><td><code>2021/7/9 13:07:04</code></td></tr> <tr><td>FF</td><td>&nbsp;</td><td>less short localized date and time with seconds</td><td><code>2021年7月9日 13:07:04</code></td></tr> <tr><td>FFF</td><td>&nbsp;</td><td>verbose localized date and time with seconds</td><td><code>2021年7月9日 13:07:04 JST</code></td></tr> <tr><td>FFFF</td><td>&nbsp;</td><td>extra verbose localized date and time with seconds</td><td><code>2021年7月9日金曜日 13時07分04秒 日本標準</code></td></tr> <tr><td>X</td><td>&nbsp;</td><td>unix timestamp in seconds</td><td><code>1625803624</code></td></tr> <tr><td>x</td><td>&nbsp;</td><td>unix timestamp in milliseconds</td><td>`1625803624054</td></tr> </tbody> </table> </figure> |

**Returns:** *string*

___

### sleep

▸ **sleep**(`ms`: *number*): *void*

指定された時間スリープします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ms` | *number* | スリープする時間（単位：ミリ秒） |

**Returns:** *void*
