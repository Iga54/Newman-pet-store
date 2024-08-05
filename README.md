# Newman API tests of Postman collection

## Project description

This project is an example of using GitHub Actions for automated API testing with Newman and Node.js. The project is configured to run tests every time code is pushed to the main branch of the repository or when a pull request is created for that branch. Before pushing the branch collection and environment in Postman were created in order to export them as a JSON files and put in the repository.

## Project configuration

1. The first step is to run a command "npm install" in console
2. Docker should be enabled on computer
3. Run command in computer terminal `docker run  --name swaggerapi-petstore3 -d -p 8080:8080 swaggerapi/petstore3:unstable` to 
4. The next issue is running scripts mentioned below:
- to run tests `npm run newman`
- to create a report from tests `npm run report`
5. Run command console within VScode `git push`

## Frameworks used in the project

1. Postman: used for creating and exporting API collections and environments.
2. Newman ^6.1.3: used to automate the execution of Postman collections. This allows for consistent and repeatable testing of APIs without manual intervention.
3. GitHub Actions: automates the execution of tests in the CI/CD pipeline.
4. Node.js: runtime environment for executing scripts.
5. Docker: runs the Petstore service in a container for API testing.

## Project documentation

Here is the official link to the Petstore documentation: https://petstore.swagger.io/#/