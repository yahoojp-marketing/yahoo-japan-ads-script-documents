# 天気 / WeatherApp

### 天気データの取得 / Get a weather data.
```.js
function getWeatherData() {
  const minatoKuWeather = WeatherApp.getWeatherByName(
                            '東京都 港区', // prefecture name or city name 
                            'TODAY' // TODAY or TOMORROW or TODAY_AND_TOMORROW
                          ); 

  const hour = minatoKuWeather[0].hour[12]; // 0: 0 o'clock、1: 1 o'clock、12:12o'clock etc..
  
  Logger.log(
    '12:00 today  ' + 
    'weather telop: ' + hour.weather.telop + '  ' + // [天気テロップ] 晴れ、曇り、雨、雪 etc..
    'precipitation: ' + hour.precip.value + hour.precip.unit + '  ' + // [降水量] XXmm etc..
    'chance of precipitation: ' + hour.probPrecip + '  ' + // [降水確率] 0、10、20、etc..
    'wind direction: ' + hour.windDirection.name + '  ' + // [風向き] 静穏、南南東、北西、etc..
    'wind speed: ' + hour.windSpeed.value + hour.windSpeed.unit + '  ' + // [風量] XXm/s etc..
    'temperature: ' + hour.temp + '  ' +  // [気温] -1、0、1、2、etc..
    'humidity: ' + hour.humidity + '  ' + // [湿度] 50、51、52 etc..
    'snowfall: ' + hour.snowFall // [降雪量] 0、1、2、etc..
  );
  
  const hour3 = minatoKuWeather[0].hour3[3]; // 0: 0:00-3:00、1: 3:00-6:00、2: 6:00-9:00 3: 9:00-12:00 etc..
  
   Logger.log(
    '9:00-12:00 today  ' + 
    'weather telop: ' + hour3.weather.telop + '  ' + // [天気テロップ] 晴れ、曇り、雨、雪 etc..
    'precipitation: ' + hour3.precip.value + hour3.precip.unit + '  ' + // [降水量] XXmm etc..
    'chance of precipitation: ' + hour3.probPrecip + '  ' + // [降水確率] 0、10、20、etc..
    'wind direction: ' + hour3.windDirection.name + '  ' + // [風向き] 静穏、南南東、北西、etc..
    'wind speed: ' + hour3.windSpeed.value + hour3.windSpeed.unit + '  ' + // [風量] XXm/s etc..
    'temperature: ' + hour3.temp + '  ' +  // [気温] -1、0、1、2、etc..
    'humidity: ' + hour3.humidity + '  ' + // [湿度] 50、51、52 etc..
    'snowfall: ' + hour3.snowFall // [降雪量] 0、1、2、etc..
  ); 
  
  const day = minatoKuWeather[0].day[0];
  
  Logger.log(
    'today  ' + 
    'weather telop: ' + day.weather.telop + '  ' + // [天気テロップ] 晴れ、曇り、雨、雪 etc..
    'maximum temperature: ' + day.temp.max + '  ' +  // [最高気温] -1、0、1、2、etc..
    'maximum temperature difference: ' + day.temp.maxDiff + '  ' +  // [最高気温前日差] -1、0、1、2、etc..
    'minimum temperature: ' + day.temp.min + '  ' +  // [最低気温] -1、0、1、2、etc..
    'minimum temperature difference: ' + day.temp.minDiff + '  ' +  // [最低気温前日差] -1、0、1、2、etc..
    'chance of precipitation: ' + day.probPrecip + '  ' + // [降水確率] 0、10、20、etc..
    'wind forecast: ' + day.wind + '  ' + // [風予測] 西の風やや強く、etc..
    'wave forecast: ' + day.wave + '  ' + // [波予測] 3メートル後2.5メートル etc..
    'sunrise time: ' + day.sunrise + '  ' +  // [日の出時間] 07:06 etc..
    'sunset time: ' + day.sunset // [日の入時間] 15:51 etc..
  );  
  
}
```
