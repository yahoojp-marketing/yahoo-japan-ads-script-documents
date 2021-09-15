# MailApp


Mail送信機能を提供するMailApp

## Table of contents

### Methods

- [sendEmail](mailapp.md#sendemail)

## Methods

### sendEmail

▸ **sendEmail**(`recipient`: *string*[], `subject`: *string*, `body`: *string*): *void*

指定された宛先にメールを送信します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `recipient` | *string*[] | 宛先となるYahoo! JAPAN ビジネスID |
| `subject` | *string* | メール件名 |
| `body` | *string* | メール本文 |

**Returns:** *void*

▸ **sendEmail**(`recipient`: *string*[], `subject`: *string*, `body`: *string*, `options`: [*MailOptions*](mailoptions.md)): *void*

指定された宛先にメールを送信します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `recipient` | *string*[] | 宛先となるYahoo! JAPAN ビジネスID |
| `subject` | *string* | メール件名 |
| `body` | *string* | メール本文 |
| `options` | [*MailOptions*](mailoptions.md) | オプション |

**Returns:** *void*

▸ **sendEmail**(`to`: *string*[], `replyTo`: *string*, `subject`: *string*, `body`: *string*): *void*

指定された宛先にメールを送信します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `to` | *string*[] | 宛先となるYahoo! JAPAN ビジネスID |
| `replyTo` | *string* | 返信先となるYahoo! JAPAN ビジネスID |
| `subject` | *string* | メール件名 |
| `body` | *string* | メール本文 |

**Returns:** *void*

▸ **sendEmail**(`message`: [*MailMessage*](mailmessage.md)): *void*

指定された宛先にメールを送信します<br>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | [*MailMessage*](mailmessage.md) | メッセージオブジェクト |

**Returns:** *void*
