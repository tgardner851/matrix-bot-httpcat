# matrix-bot-httpcat
A matrix bot to retrieve pictures of cats for HTTP status codes

# Usage

1. Invite bot to a private room
2. Send a message `!httpcat [HTTP STATUS CODE]` to get a response

# Building your own

*Note*: You'll need to have access to an account that the bot can use to get the access token.

1. Clone this repository
2. `npm install`
3. `npm run build`
4. Copy `config/default.yaml` to `config/production.yaml`
5. Run the bot with `NODE_ENV=production node lib/index.js`

### Docker

```
A Dockerfile and docker-compose are provided.

Build the docker image:
`docker build -t matrix-bot-httpcat .`

Build the docker image and run docker-compose to deploy to your server:
`docker build -t matrix-bot-httpcat . && docker-compose run matrix-bot-httpcat`
```
