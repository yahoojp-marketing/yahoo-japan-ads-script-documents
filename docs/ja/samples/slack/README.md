# Slack

### メッセージを投稿する / Post a message

```
function sendSlackMessage(){
  UrlFetchApp.fetch('http://<Your Incoming Webhook URL>',
  {
    method: 'POST',
    contentType: 'application/json',
    payload: {
      'text': `
        Hello, world.
        http://yahoo.co.jp/
        :cat:`, //specify stamps in English
      icon_url: 'https://xxx.com/icon_400x400.jpg',
      username: 'YOUR_USER_NAME',
      channel: 'YOUR_CHANNEL_ID'
    }
  });
}
```
