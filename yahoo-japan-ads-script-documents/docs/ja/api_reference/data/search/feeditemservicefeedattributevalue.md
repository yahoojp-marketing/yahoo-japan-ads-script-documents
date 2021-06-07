# FeedItemServiceFeedAttributeValue


<div lang=\"ja\">FeedItemServiceFeedAttributeValueオブジェクトは、フィードアイテムの属性値を表示します。<br> 更新時にfeedAttributeValueを指定するとすべて上書きされ、未指定のfeedAttributeValueの属性情報は削除されます。<br> feedAttributeValueに空文字を指定すると、下記の場合のみフィードアイテムの属性情報は削除されます。   <table border=\"1\">     <thead>       <tr>         <th>placeholderType</th>         <th>placeholderField</th>       </tr>     </thead>     <tbody>       <tr>         <td>QUICKLINK</td>         <td>ADVANCED_MOBILE_URL</td>       </tr>       <tr>         <td>QUICKLINK</td>         <td>TRACKING_URL</td>       </tr>       <tr>         <td>AD_CUTOMIZER</td>         <td>any</td>       </tr>     </tbody>   </table> </div> 

## Table of contents

### Properties

- [disapprovalReasonCodes](feeditemservicefeedattributevalue.md#disapprovalreasoncodes)
- [feedAttributeValue](feeditemservicefeedattributevalue.md#feedattributevalue)
- [reviewFeedAttributeValue](feeditemservicefeedattributevalue.md#reviewfeedattributevalue)

## Properties

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査の否認理由コードです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** FeedItemServiceFeedAttributeValue

___

### feedAttributeValue

• `Optional` **feedAttributeValue**: ``null`` \| *string*

<div lang=\"ja\">フィードアイテムの属性値です。<br> このフィールドは、ADDおよびSET時に必須となり、REMOVE時は無視されます。</div> 

**`memberof`** FeedItemServiceFeedAttributeValue

___

### reviewFeedAttributeValue

• `Optional` **reviewFeedAttributeValue**: ``null`` \| *string*

<div lang=\"ja\">レビュー中のフィードアイテムの属性値です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** FeedItemServiceFeedAttributeValue
