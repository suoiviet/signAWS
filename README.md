# Python AWS 4 Signing
This python script calls a REST api hosted on AWS Api Gateway with Authorization set to AWS IAM.

When a REST api has Authorization set to AWS IAM, the calling script needs to authenticate by AWS Version 4 Signing. This requires the client to pass in valid AWS keys (access & secret keys) when calling the api.

This script assumes you are calling the api endpoint 'https://zzzyyyxxxuuu.execute-api.us-east-1.amazonaws.com/prod/rest-endpoint' in which the endpoint expects two request parameters ("startdate" & "enddate") in the payload. We will be calling using the POST method.


## Executing the csript
1. Make sure you have these installed
	- Python

## More Stuff
See: http://docs.aws.amazon.com/general/latest/gr/sigv4_signing.html