# Subscriptions

A resource function with the `subscribe` accessor inside a GraphQL service
represents a field in the root `Subscription` object type. Therefore, if a
resource function with the `subscribe` accessor is present inside the
Ballerina GraphQL service, the auto-generated schema will have a `Subscription`
type. <br/><br/>
Each resource function with the `subscribe` accessor in the service will
be added as a field of the `Subscription` type. The field name will be the
resource function name, and the field type will be the constraint type of
the stream returned from the resource function.
<br/><br/>
For more information on the underlying package, see the
[GraphQL package](https://docs.central.ballerina.io/ballerina/graphql/latest/).

::: code graphql_subscriptions.bal :::

::: out graphql_subscriptions.client.out :::

::: out graphql_subscriptions.server.out :::