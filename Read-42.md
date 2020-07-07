## Nextjs Deployment
- The easiest way to deploy Next.js to production is to use the Vercel platform
- Vercel supports the DPS workflow: Develop, Preview, and Ship 
- Every page can either use Static Generation or Server-Side Rendering.
- Pages that use Static Generation and assets (JS, CSS, images, fonts, etc) will automatically be served from the Vercel Smart CDN, which is blazingly fast.
- Pages that use Server-Side Rendering and API routes will automatically become isolated Serverless Functions. This allows page rendering and API requests to scale infinitely.

## Elephant SQL
- ElephantSQL automates every part of setup and running of PostgreSQL clusters.
- Automated backups are performed every day, which is stored in a cloud file storage so that they are always accessible to you. You can also use point-in-time-recovery to restore your database
- ElephantSQL installs and manages PostgreSQL databases for you
- SaaS option for PostgreSQL that have support for streaming replication across clouds. 
- ElephantSQL provides a browser tool for SQL queries where you can create, read, update and delete data directly from your web browse 

## Docker on Heroku
- The heroku.yml file is a manifest you can use to define your Heroku app. It allows you to:
    - Build Docker images on Heroku
    - Specify add-ons and config vars to create during app provisioning
    - Take advantage of Review Apps when deploying Docker-based applications
- Create a heroku.yml file in your application’s root directory.
- Commit the file to your repo:
``
git add heroku.yml
git commit -m "Add heroku.yml"
``
- Set the stack of your app to container:
``
heroku stack:set container
``
- Push your app to Heroku:
``
git push heroku master
``

- A heroku.yml manifest has 4 top-level sections:
    - setup - Specifies the add-ons and config vars to create during app provisioning
    - build - Specifies the Dockerfile to build
    - release - Specifies the release phase tasks to execute
    - run - Specifies process types and the commands to run for each