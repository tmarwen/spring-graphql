**GraphQL WebSocket Endpoint with Spring WebFlux**

 - [Data Controller](src/main/java/io/spring/sample/graphql/SampleController.java) with reactive methods for queries and subscriptions.
 - [WebFilter](src/main/java/io/spring/sample/graphql/ContextWebFilter.java) to insert Reactor `Context` and check it can be accessed in [DataRepository](src/main/java/io/spring/sample/graphql/DataRepository.java).
 - Subscription [tests](src/test/java/io/spring/sample/graphql/SubscriptionTests.java) using Reactor's `StepVerifier` to verify the stream.
 
 GraphiQL does not support subscriptions. There is a basic index.html page that logs subscriptions the console.