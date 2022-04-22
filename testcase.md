##Feature: Individual account login

Scenario 1: Login with signature

Given I generate access token of admin by x-api-key.
And I create individual account with access token of Admin.
And I convert secret key to signature key.
When I send request to generate access token by signature.
And I use signature in header of request
And I use access token of Admin in authorization option.
Then I see the response of request is displayed.
And I see the status of response is 200 OK
And I see the success property is TRUE.
And I see the data object has access-token property.
And I see the access-token object is not null

##Feature: Organization account login

Scenario 2: Login with signature

Given I generate access token of admin by x-api-key.
And I create individual account with access token of Admin.
And I convert secret key to signature key.