# SwaggerClient::DefaultApi

All URIs are relative to *https://api.pbxdom.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**calls_get**](DefaultApi.md#calls_get) | **GET** /Calls | 
[**features_charts_get**](DefaultApi.md#features_charts_get) | **GET** /Features/charts | 
[**features_reports_get**](DefaultApi.md#features_reports_get) | **GET** /Features/reports | 
[**features_widget_get**](DefaultApi.md#features_widget_get) | **GET** /Features/widget | 


# **calls_get**
> Array&lt;InlineResponse200&gt; calls_get(rpt_type, rpt_id, opts)



Gets `Calls` info. 

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

rpt_type = 1.2 # Float | Report type. (0 report, 1 widget, 2 chart).

rpt_id = 1.2 # Float | Report id.

opts = { 
  start: 3.4, # Float | Start offset.
  limit: 3.4, # Float | Number of results to return. Max 10K.
  sort_by: "sort_by_example", # String | Sort column.
  sort_type: "sort_type_example", # String | Sort mode asc/desc.
  from_date: "from_date_example", # String | Start date time.
  to_date: "to_date_example", # String | End date time.
  duration: 3.4, # Float | Duration range.
  phone: "phone_example", # String | List of caller phone.
  phone1: "phone1_example", # String | List of dialled phones.
  co: "co_example", # String | List of trunk/co.
  ext: "ext_example", # String | list of extensions.
  pbx_id: 3.4, # Float | list of PBX Ids.
  call_source: 3.4, # Float | list of callsource.
  call_type: 3.4, # Float | list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls)
  direction: 3.4, # Float | list of direction.(0 incoming, 1 outgoing, 2 internal)
  caller_name: "caller_name_example", # String | list of caller name.
  did: "did_example", # String | list of did.
  dnis: "dnis_example", # String | list of dnis.
  acc: "acc_example", # String | list of account code.
  ring: 3.4, # Float | Ring range.Seconds unit.
  cost: 3.4, # Float | Cost range.
  group: 3.4 # Float | Department/Group id.
}

begin
  result = api_instance.calls_get(rpt_type, rpt_id, opts)
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->calls_get: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rpt_type** | **Float**| Report type. (0 report, 1 widget, 2 chart). | 
 **rpt_id** | **Float**| Report id. | 
 **start** | **Float**| Start offset. | [optional] 
 **limit** | **Float**| Number of results to return. Max 10K. | [optional] 
 **sort_by** | **String**| Sort column. | [optional] 
 **sort_type** | **String**| Sort mode asc/desc. | [optional] 
 **from_date** | **String**| Start date time. | [optional] 
 **to_date** | **String**| End date time. | [optional] 
 **duration** | **Float**| Duration range. | [optional] 
 **phone** | **String**| List of caller phone. | [optional] 
 **phone1** | **String**| List of dialled phones. | [optional] 
 **co** | **String**| List of trunk/co. | [optional] 
 **ext** | **String**| list of extensions. | [optional] 
 **pbx_id** | **Float**| list of PBX Ids. | [optional] 
 **call_source** | **Float**| list of callsource. | [optional] 
 **call_type** | **Float**| list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls) | [optional] 
 **direction** | **Float**| list of direction.(0 incoming, 1 outgoing, 2 internal) | [optional] 
 **caller_name** | **String**| list of caller name. | [optional] 
 **did** | **String**| list of did. | [optional] 
 **dnis** | **String**| list of dnis. | [optional] 
 **acc** | **String**| list of account code. | [optional] 
 **ring** | **Float**| Ring range.Seconds unit. | [optional] 
 **cost** | **Float**| Cost range. | [optional] 
 **group** | **Float**| Department/Group id. | [optional] 

### Return type

[**Array&lt;InlineResponse200&gt;**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined



# **features_charts_get**
> Array&lt;InlineResponse200&gt; features_charts_get



Gets `Charts` list. 

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

begin
  result = api_instance.features_charts_get
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->features_charts_get: #{e}"
end
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Array&lt;InlineResponse200&gt;**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined



# **features_reports_get**
> Array&lt;InlineResponse200&gt; features_reports_get



Gets `Reports` list. 

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

begin
  result = api_instance.features_reports_get
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->features_reports_get: #{e}"
end
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Array&lt;InlineResponse200&gt;**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined



# **features_widget_get**
> Array&lt;InlineResponse200&gt; features_widget_get



Gets `Widgets` list. 

### Example
```ruby
# load the gem
require 'swagger_client'

api_instance = SwaggerClient::DefaultApi.new

begin
  result = api_instance.features_widget_get
  p result
rescue SwaggerClient::ApiError => e
  puts "Exception when calling DefaultApi->features_widget_get: #{e}"
end
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Array&lt;InlineResponse200&gt;**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined



