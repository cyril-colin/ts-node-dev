# ts-node-dev
A simple docker to run ts-node-dev into a docker container.

You can see the ts-node-dev documentation to the [npm repository](https://www.npmjs.com/package/ts-node-dev)

## Usage sample

```bash
docker run -t \
  --name ts-node-dev \
  -v "./path-to-sources":/workdir \
  -p 3000:3000 \
  --rm coyotetuba/ts-node-dev \
  bash -c "ts-node-dev --project \"/workdir/tsconfig.json\"  \"/workdir/server.ts\""
```


## Why

I have created this image in order to run my project in a dev environment easily in docker. You can
checkout my project and see a more complex usage of this image to the [Tohr](https://github.com/cyril-colin/tohr) project.
