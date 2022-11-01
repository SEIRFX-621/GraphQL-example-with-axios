# prerequisite reading

If you're choosing to use a graphql API in your project, please familiarize yourself with the basic of graphql.

Read intro to graphql: [GraphQL introduction](https://graphql.org/)

# Setup for this example

This example uses axios only. be sure to run `npm i` before running the project.

This example uses the podchaser graphql API: [Podchaser GraphQL API](https://api-docs.podchaser.com)

You will need to create an account and generate an API secret and an API key, once completed, create an .env file in this project and ass the values to CLIENT_KEY and CLIENT_SECRET, these are used in the example. 

to setup authorization, follow these doc [Podchaser Authorization](https://api-docs.podchaser.com/docs/authorization)
for api documentation, use these docs as an example to create your queries [Poschase API docs](https://api-docs.podchaser.com/docs/overview)

## Rate limit in Podchaser

Podchaser doesn't limit usage by individual requests, but it limits usage by fields pulled in your queries. Please see their documentation on how you will be billed [Podchase rate limits](https://api-docs.podchaser.com/docs/rate-limits)

you have a limit of 25,000 points on their free tier, this means you can pull 25,000 individual fields from their api, their documentation explains this in more detail. 

# Debugging

I have added a vs code launch.json file for easy debugging using vs code. You can find this in ./vscode/launch.json location.