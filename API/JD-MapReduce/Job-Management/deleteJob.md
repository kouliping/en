# deleteJob


## 描述
Delete a job specified by jobId

## 请求方式
POST

## 请求地址
https://idata-jmr-api.jcloud.com/v1/regions/{regionId}/job/{jobId}:delete

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**jobId**|String|True||Job Id to be deleted|
|**regionId**|String|True||Region ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String||
|**result**|[Result](##Result)||


### <a name="Result">Result</a>
|名称|类型|描述|
|---|---|---|
|**message**|String||
|**status**|String||

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**500**|Internal server error|
