# CampaignServiceTargetSpendBiddingScheme


<div lang=\"ja\">CampaignServiceTargetSpendBiddingSchemeオブジェクトは、クリック数の最大化の自動入札設定情報を表します。（BiddingStrategyService以外用のオブジェクトです。）<br> ADD時、BiddingStrategyTypeがTARGET_SPENDの場合、必須となり、それ以外では省略可能となります。</div> 

## Table of contents

### Properties

- [bidCeiling](campaignservicetargetspendbiddingscheme.md#bidceiling)

## Properties

### bidCeiling

• `Optional` **bidCeiling**: ``null`` \| *number*

<div lang=\"ja\">入札価格の上限です。<br>※「0」が設定された 場合、上限設定は ありません。<br> このフィールドは省略可能となります。その際、デフォルト設定値は0となります。</div> 

**`memberof`** CampaignServiceTargetSpendBiddingScheme
