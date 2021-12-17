# ForecastWeather


天気を表すオブジェクトです。<br>
天気を表すテロップと、天気詳細を表す以下の天気コードで構成されています。
<p>&nbsp;</p>
<figure>
<table>
<caption>1日天気の天気コード対応表</caption>
<thead>
<tr><th>天気コード</th><th>天気詳細</th></tr>
</thead>
<tbody>
<tr><td>100</td><td>晴れ</td></tr>
<tr><td>101</td><td>晴時々曇</td></tr>
<tr><td>102</td><td>晴一時雨</td></tr>
<tr><td>103</td><td>晴時々雨</td></tr>
<tr><td>104</td><td>晴一時雪</td></tr>
<tr><td>105</td><td>晴時々雪</td></tr>
<tr><td>111</td><td>晴のち曇</td></tr>
<tr><td>114</td><td>晴のち雨</td></tr>
<tr><td>117</td><td>晴のち雪</td></tr>
<tr><td>119</td><td>晴のち雨で雷を伴う</td></tr>
<tr><td>140</td><td>晴時々雨で雷を伴う</td></tr>
<tr><td>149</td><td>晴のち雪で雷を伴う</td></tr>
<tr><td>150</td><td>晴時々雪で雷を伴う</td></tr>
<tr><td>156</td><td>晴時々黒くも</td></tr>
<tr><td>158</td><td>晴時々黒くもりで雷を伴う</td></tr>
<tr><td>166</td><td>晴れのち曇</td></tr>
<tr><td>168</td><td>晴のち黒くもりで雷を伴う</td></tr>
<tr><td>200</td><td>曇り</td></tr>
<tr><td>201</td><td>曇時々晴</td></tr>
<tr><td>202</td><td>曇一時雨</td></tr>
<tr><td>203</td><td>曇時々雨</td></tr>
<tr><td>204</td><td>曇一時雪</td></tr>
<tr><td>205</td><td>曇時々雪</td></tr>
<tr><td>211</td><td>曇のち晴</td></tr>
<tr><td>214</td><td>曇のち雨</td></tr>
<tr><td>217</td><td>曇のち雪</td></tr>
<tr><td>219</td><td>曇のち雨で雷を伴う</td></tr>
<tr><td>240</td><td>曇時々雨で雷を伴う</td></tr>
<tr><td>249</td><td>曇のち雪で雷を伴う</td></tr>
<tr><td>250</td><td>曇時々雪で雷を伴う</td></tr>
<tr><td>255</td><td>曇り</td></tr>
<tr><td>257</td><td>曇で雷を伴う</td></tr>
<tr><td>258</td><td>曇で雷を伴い時々晴</td></tr>
<tr><td>266</td><td>曇のち晴</td></tr>
<tr><td>268</td><td>曇で雷を伴いのち晴</td></tr>
<tr><td>300</td><td>雨</td></tr>
<tr><td>301</td><td>雨時々晴</td></tr>
<tr><td>302</td><td>雨時々曇</td></tr>
<tr><td>311</td><td>雨のち晴</td></tr>
<tr><td>313</td><td>雨のち曇</td></tr>
<tr><td>315</td><td>雨のち雪</td></tr>
<tr><td>330</td><td>雨時々雪</td></tr>
<tr><td>341</td><td>雨で雷を伴いのち晴</td></tr>
<tr><td>343</td><td>雨で雷を伴いのち曇</td></tr>
<tr><td>345</td><td>雨で雷を伴いのち雪</td></tr>
<tr><td>350</td><td>雨で雷を伴う</td></tr>
<tr><td>400</td><td>雪</td></tr>
<tr><td>401</td><td>雪時々晴</td></tr>
<tr><td>402</td><td>雪時々曇</td></tr>
<tr><td>411</td><td>雪のち晴</td></tr>
<tr><td>413</td><td>雪のち曇</td></tr>
<tr><td>414</td><td>雪のち雨</td></tr>
<tr><td>441</td><td>雪で雷を伴いのち晴</td></tr>
<tr><td>443</td><td>雪で雷を伴いのち曇</td></tr>
<tr><td>444</td><td>雪で雷を伴いのち雨</td></tr>
<tr><td>450</td><td>雪で雷を伴う</td></tr>
<tr><td>500</td><td>大雨</td></tr>
<tr><td>550</td><td>大雨で雷を伴う</td></tr>
<tr><td>600</td><td>大雪</td></tr>
<tr><td>650</td><td>大雪で雷を伴う</td></tr>
<tr><td>700</td><td>暴風雨</td></tr>
<tr><td>750</td><td>暴風雨で雷を伴う</td></tr>
<tr><td>800</td><td>暴風雪</td></tr>
<tr><td>850</td><td>暴風雪で雷を伴う</td></tr>
</tbody>
</table>
</figure>

<p>&nbsp;</p>
<figure>
<table>
<caption>1h/3h天気の天気コード対応表</caption>
<thead>
<tr><th>天気コード</th><th>天気詳細</th></tr>
</thead>
<tbody>
<tr><td>10</td><td>快晴</td></tr>
<tr><td>20</td><td>白雲多めの晴れ</td></tr>
<tr><td>21</td><td>黒雲多めの晴れ</td></tr>
<tr><td>30</td><td>曇り</td></tr>
<tr><td>31</td><td>黒曇り</td></tr>
<tr><td>34</td><td>曇りで雷を伴う</td></tr>
<tr><td>41</td><td>降ったり止んだりなどの弱い雨</td></tr>
<tr><td>43</td><td>降ったり止んだりなどの弱い雪</td></tr>
<tr><td>51</td><td>雨</td></tr>
<tr><td>52</td><td>みぞれ</td></tr>
<tr><td>53</td><td>雪</td></tr>
<tr><td>54</td><td>雨で雷を伴う</td></tr>
<tr><td>56</td><td>雪で雷を伴う</td></tr>
<tr><td>61</td><td>強雨</td></tr>
<tr><td>63</td><td>大雪</td></tr>
<tr><td>64</td><td>強雨で雷を伴う</td></tr>
<tr><td>66</td><td>大雪で雷を伴う</td></tr>
<tr><td>81</td><td>暴風雨</td></tr>
<tr><td>83</td><td>暴風雪</td></tr>
<tr><td>84</td><td>暴風雨で雷を伴う</td></tr>
<tr><td>86</td><td>暴風雪で雷を伴う</td></tr></tbody>
</table>
</figure>

## Table of contents

### Properties

- [code](forecastweather.md#code)
- [telop](forecastweather.md#telop)

## Properties

### code

• **code**: *number*

天気予報コード

___

### telop

• **telop**: *string*

天気予報テロップ
