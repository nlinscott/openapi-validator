### openapi-validator

An API used to validate client side models against the server that requires them.

## Problem

Server side models in the form of code cant always be shared with its client. This is usually because of language differences. C# models cannot be used by an angular or nodejs frontend.

## Solution

These services allow you to send a sample request using the models the client expects and then verifies that the request is valid based on the OpenAPI specification the server uses.
If valid, a fully-formed sample response is sent back. The client is then able to evaluate the response and make sure the models they are using are correct.

Calls to this service should be made as part of your automation efforts. Production systems typically do not publish their OpenAPI specs.

