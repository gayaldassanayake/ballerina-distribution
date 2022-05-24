# Error Handling

Error handling is an integral part of any network program. Errors can be returned
by many components such as interceptors, dispatcher, data-binder, security handlers, etc.
These errors are often handled by a default handler and sent back as error responses
with an entity-body. With the introduction of error interceptors, you can intercept 
these errors and handle them as you wish. These error interceptors can be placed 
anywhere in the interceptor pipeline. When there is an error, the execution jumps
to the closest error interceptor.
For more information, see the [`http` module](https://docs.central.ballerina.io/ballerina/http/latest/).

::: code ./examples/http-error-handling/http_error_handling.bal :::

::: out ./examples/http-error-handling/http_error_handling.client.out :::

::: out ./examples/http-error-handling/http_error_handling.server.out :::