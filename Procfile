web:    WEB_SERVER=true  SCHEDULER=true  WORKERS=1  cd node_modules/@grouparoo/core && ./api/bin/start
worker: WEB_SERVER=false SCHEDULER=true  WORKERS=10 cd node_modules/@grouparoo/core && ./api/bin/start

# Note: Normally, `web` would have no workers or scheduler, but we want to be able to run the app on a simple heroku deploy
