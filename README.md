# Python AWS 4 Signing
This python script calls a REST api hosted on AWS Api Gateway with Authorization set to AWS IAM.

When a REST api has Authorization set to AWS IAM, the calling script needs to authenticate by AWS Version 4 Signing. This requires the client to pass in valid AWS keys (access & secret keys) when calling the api.

This script assumes you are calling the api endpoint 'https://zzzyyyxxxuuu.execute-api.us-east-1.amazonaws.com/prod/rest-endpoint' in which the endpoint expects two request parameters ("startdate" & "enddate") in the payload. We will be calling using the POST method.


## Executing the script
1. Make sure you have these installed
	- Python
2. Open signAWS.py with a text editor: 
	- Enter valid dates for the "startdate" & "enddate" (in YYYYMMDD format)
	- Make sure "endpoint" variable is pointing to a valid url
	- Make sure all variables in the REQUEST VALUES section are poitning to your own AWS API Gateway endpoint
	- Provide your own AWS keys (access & secret keys) under the "Read AWS access key" section
3. Open Terminal and change the directory to the location of signAws.py. Run signAWS.py

## More Stuff
See: http://docs.aws.amazon.com/general/latest/gr/sigv4_signing.html