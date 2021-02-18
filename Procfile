web:    cd node_modules/@grouparoo/core && WEB_SERVER=true  WORKERS=1  ./api/bin/start
worker: cd node_modules/@grouparoo/core && WEB_SERVER=false WORKERS=10 ./api/bin/start

# Note: Normally, `web` would have no workers or scheduler, but we want to be able to run the app on a simple heroku deploy
