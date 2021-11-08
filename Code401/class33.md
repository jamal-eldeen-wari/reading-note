## Importance of using API (GRAPHQL):
It is used to enhance your your schema with additional capabilities such as custom indexes, authorization rules, function triggers, and much more.

What are the AWS AppSync-provided directives??
A: can be used within the Amplify GraphQL schemas. These will not be processed by Amplify CLI but passed through to the service as is and will be present in the output schema. For instance:
1. @aws_api_key
2. @aws_iam
3. @aws_oidc
4. @aws_cognito_user_pools
5. @aws_auth
6. m@aws_subscribe

Also There are some 3rd Party Directives such as:
1. @algolia: Adds serverless search to your Amplify API with Algolia
2. @ttl: Enables DynamoDB's time-to-live feature to auto-delete old entries in your AWS Amplify API
3. @firehose: Adds a simple interceptor to all of your Amplify API mutations and queries
4. @retain: Enables the **Retain** deletion policy for your Amplify-generated DynamoDB tables.


# @connection:
It  enables you to specify relationships between **@model** types. Currently, this supports one-to-one, one-to-many, and many-to-one relationships. You may implement many-to-many relationships using two one-to-many connections and a joining **@model** type.

Where can we use @Connection??
A: It can be used by annotating fields on an @model object type with the @connection directive.


The fields argument can be provided and indicates which fields can be queried by to get connected objects. The keyName argument can optionally be used to specify the name of secondary index (an index that was set up using @key) that should be queried from the other type in the relationship.

When specifying a keyName, the fields argument should be provided to indicate which field(s) will be used to get connected objects. If keyName is not provided, then @connection queries the target table's primary index.

Here are Some of the Relations:
1. Has One: you can define a one-to-one connection where a project has one team.Where you can also define the field you would like to use for the connection by populating the first argument to the fields array and matching it to a field on the type.

2. Has many: Note how a one-to-many connection needs an @key that allows comments to be queried by the postID and the connection uses this key to get all comments whose postID is the id of the post was called on. After it's transformed.

3. Belongs to: it allows us to  make a connection bi-directional by adding a many-to-one connection to types that already have a one-to-many connection. In this case you add a connection from Comment to Post since each comment belongs to a post.

4. Many-to-many connections: You can implement many to many using two 1-M @connections, an @key, and a joining @model.