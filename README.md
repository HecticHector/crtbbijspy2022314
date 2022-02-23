crtbbijspy2022314

## \_\_1

npmjs.com/package/wscat
wscat -c wss://stream.binance.com:9443/ws/btcusdt@trade

< {"e":"trade","E":1645602972064,"s":"BTCUSDT","t":1265639946,"p":"38136.60000000","q":"0.00200000","b":9503230859,"a":9503232490,"T":1645602972064,"m":true,"M":true}

## \_\_2

github.com/binance/binance-spot-api-docs/blob/master/web-socket-streams.md
The base endpoint is: wss://stream.binance.com:9443
Raw streams are accessed at /ws/<streamName>

## \_\_3

github.com/binance/binance-spot-api-docs/blob/master/web-socket-streams.md#klinecandlestick-streams
Stream Name: <symbol>@kline\_<interval>
wscat -c wss://stream.binance.com:9443/ws/btcusdt@kline_15m

< {"e":"kline","E":1645603361891,"s":"BTCUSDT","k":{
"t":1645603200000,"T":1645604099999,"s":"BTCUSDT","i":"15m","f":1265642384,"L":1265644498,"o":"38151.16000000","c":"38179.09000000","h":"38188.98000000","l":"38116.45000000","v":"84.49121000","n":2115,"x":false,"q":"3223459.45854370","V":"38.35880000","Q":"1463375.36537200","B":"0"}
}

wscat -c wss://stream.binance.com:9443/ws/btcusdt@kline_15m | tee dataset.txt

## \_\_4

developer.mozilla.org/en-US/docs/Web/API/WebSockets_API/Writing_WebSocket_client_applications
var exampleSocket = new WebSocket("wss://www.example.com/socketserver", "protocolOne");

## \_\_5

github.com/tradingview/lightweight-charts
npm install lightweight-charts
or
https://unpkg.com/lightweight-charts/dist/lightweight-charts.standalone.production.js

## \_\_6

tradingiview.com/lightweight-charts/
jsfiddle.net/TradingView/eaod9Lq8/
