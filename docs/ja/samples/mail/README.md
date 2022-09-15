# メール / Mail

### 簡単なメールを送信する / Send a simple email
```.js
function sendSimpleEmail(){
 
  MailApp.sendEmail({
    to: ['<Yahoo! JAPAN Business ID>'], //write one or more.
    subject: '<SIMPLE_MAIL_TITLE>',
    body: '<SIMPLE_MAIL_BODY>',
  });
   
}
```

### HTMLメールを送信する / Send HTML email
```.js
function sendHtmlEmail(){
 
  //Multiple can be specified
  const toArray = ['<Yahoo! JAPAN Business ID>']; //write one or more.
  const ccArray = []; //zero or more
  const bccArray = []; //zero or more
 
  const mailTitle = '<HTML_MAIL_TITLE>';
   
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const campaigns = Search.CampaignService.get({
    accountId: accountId,
  }).rval;
 
  let mailBody = 'no body';
 
  if (campaigns.values.length > 0){
    mailBody = 'All campaigns are listed below.';
    mailBody = mailBody + '<table border=\'1\'><tr><td>campaignId</td><td>campaignName</td></tr>';
     
    for (let i = 0; i < campaigns.values.length; i++){   
      let campaign = campaigns.values[i].campaign;
 
      mailBody = mailBody + '<tr><td>' 
        + campaign.campaignId + '</td><td>' 
        + campaign.campaignName + '</td></tr>';
    }
     
    mailBody = mailBody + '</table>';
  }
   
  const accounts = Search.AccountService.get({
    accountIds: [
      accountId,
    ],
  }).rval;
   
  let message =  {
    to: toArray,
    cc: ccArray,
    bcc: bccArray,
    subject: mailTitle,
    replyTo: accounts.authorizationBusinessId,
    htmlBody: mailBody,
  };
   
  MailApp.sendEmail(message);
   
}
```
