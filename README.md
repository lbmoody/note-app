# note-app
Node/Express application that can be used to write, save, and delete notes.

## installation
This application uses 2 npm packages [express](https://www.npmjs.com/package/express) to expediate the node server and [uuid](https://www.npmjs.com/package/uuid) to generate unique ids for each note. After downloading the project please run `npm i` or `npm install` to download these dependancies.

To run the applicaiton locally run `node server.js` in your command prompt of the applications local repository.

## usage
This application is used to write notes to a json file. Users can click on the list of previous notes on the left column and continue or edit existing notes. New notes can also be created by clicking the pencil in the top left. Also any notes that the user is finished with can be deleted by clicking the red trash can that correlates to a specific note. But be warned, deleting a note deletes it for good! 

Landing Page:
![image](https://user-images.githubusercontent.com/24512590/73115746-746eb000-3ee7-11ea-8132-8aefbdbdd6a7.png)

Note Page:
![image](https://user-images.githubusercontent.com/24512590/73115754-923c1500-3ee7-11ea-92d7-003eb46f444c.png)

## docker deployment with heroku
With this applicaiton I am testing containerized deployments on heroku with docker and a heroku.yml file. Since there isnt a database with this application it is just a trial run to understand and practice building docker files locally and testing deployments via docker.

If you have docker installed locally you can test the application build and run the application locally through docker. [Heroku](https://devcenter.heroku.com/categories/deploying-with-docker) Documentation to deploy with docker.


Build docker file command
`docker build -t <app-name> .`

After successful build run this command to run application locally with docker.
`docker run --rm -it -p 8080:8080 <app-name>`