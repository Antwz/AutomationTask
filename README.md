Environment: java version 11

In order to run tests run the following commands:
1. Clone the repo
2. Open command line from the project root directory
3. Run 'gradle clean test'
4. Run 'gradle allureReport' (in case of any error just ignore it)
5. Run 'gradle allureServe'
As a result test run report should be generated and opened in a browser
![image](https://user-images.githubusercontent.com/18191661/208615832-fc5fe8a8-8c06-4486-8b74-889c412a754e.png)
To see test details please open 'Suites' tab and expand the test
![image](https://user-images.githubusercontent.com/18191661/208616011-b5ee6ffd-0479-48ad-8417-8252ff30c1ff.png)

To run tests in Docker do the following:
1. Install Docker engine
2. Run 'gradle clean test -Dconfig=docker'
As a result tests should be executed inside docker image (starts automatically)
Also after running tests in conainer a new recording will be saved in the root directory of the project
![image](https://user-images.githubusercontent.com/18191661/208643462-3d4bd7c5-2185-437c-94e9-ed232b8a7670.png)
