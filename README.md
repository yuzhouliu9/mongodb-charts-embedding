# mongodb-charts-embedding
MongoDB Charts Embedding Example taken from https://github.com/mongodb-js/charts-embed-sdk/tree/master/examples/dashboard/unauthenticated with fixes and changes to make it show my dashboard for kanopy cost and efficiency.

## Steps to run
Follow these instructions on your MongoDB Chart dashboard https://www.mongodb.com/docs/charts/embed-chart-anon-auth/#std-label-anon-embedding-charts. Make sure "Allowed filter fields" is set to all.

Install nvm https://github.com/nvm-sh/nvm

Use nvm to install node `v18`, compatible with this example. Run `nvm install 18` `nvm use 18`.

Run `npm install`, `npm start`.

## Run as container
```
docker build . -t node-web-app

docker run -p 1234 node-web-app

docker ps  // Get the assigned Port number, and visit localhost:<port number> to see app
```

From this can easily be built into kanopy app
