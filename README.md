# [Backstage](https://backstage.io)

This is your newly scaffolded Backstage App, Good Luck!

To start the app, run:

```sh
yarn install
yarn dev
```

Publish app

```
docker build . -f packages/backend/Dockerfile -t registry.heroku.com/pubdev-backstage/web
heroku container:login
docker push registry.heroku.com/pubdev-backstage/web
heroku container:release web -a pubdev-backstage
```

Open: https://pubdev-backstage.herokuapp.com/