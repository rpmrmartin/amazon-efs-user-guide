# DeleteAccessPoint<a name="API_DeleteAccessPoint"></a>

Deletes the specified access point\. After deletion is complete, new clients can no longer connect to the access points\. Clients connected to the access point at the time of deletion will continue to function until they terminate their connection\.

This operation requires permissions for the `elasticfilesystem:DeleteAccessPoint` action\.

## Request Syntax<a name="API_DeleteAccessPoint_RequestSyntax"></a>

```
DELETE /2015-02-01/access-points/AccessPointId HTTP/1.1
```

## URI Request Parameters<a name="API_DeleteAccessPoint_RequestParameters"></a>

The request uses the following URI parameters\.

 ** [AccessPointId](#API_DeleteAccessPoint_RequestSyntax) **   <a name="efs-DeleteAccessPoint-request-AccessPointId"></a>
The ID of the access point that you want to delete\.  
Length Constraints: Maximum length of 128\.  
Pattern: `^(arn:aws[-a-z]*:elasticfilesystem:[0-9a-z-:]+:access-point/fsap-[0-9a-f]{8,40}|fsap-[0-9a-f]{8,40})$`   
Required: Yes

## Request Body<a name="API_DeleteAccessPoint_RequestBody"></a>

The request does not have a request body\.

## Response Syntax<a name="API_DeleteAccessPoint_ResponseSyntax"></a>

```
HTTP/1.1 204
```

## Response Elements<a name="API_DeleteAccessPoint_ResponseElements"></a>

If the action is successful, the service sends back an HTTP 204 response with an empty HTTP body\.

## Errors<a name="API_DeleteAccessPoint_Errors"></a>

 ** AccessPointNotFound **   
Returned if the specified `AccessPointId` value doesn't exist in the requester's AWS account\.  
HTTP Status Code: 404

 ** BadRequest **   
Returned if the request is malformed or contains an error such as an invalid parameter value or a missing required parameter\.  
HTTP Status Code: 400

 ** InternalServerError **   
Returned if an error occurred on the server side\.  
HTTP Status Code: 500

## See Also<a name="API_DeleteAccessPoint_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [AWS Command Line Interface](https://docs.aws.amazon.com/goto/aws-cli/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for \.NET](https://docs.aws.amazon.com/goto/DotNetSDKV3/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for Java V2](https://docs.aws.amazon.com/goto/SdkForJavaV2/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for JavaScript](https://docs.aws.amazon.com/goto/AWSJavaScriptSDK/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for PHP V3](https://docs.aws.amazon.com/goto/SdkForPHPV3/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for Python](https://docs.aws.amazon.com/goto/boto3/elasticfilesystem-2015-02-01/DeleteAccessPoint) 
+  [AWS SDK for Ruby V3](https://docs.aws.amazon.com/goto/SdkForRubyV3/elasticfilesystem-2015-02-01/DeleteAccessPoint) 