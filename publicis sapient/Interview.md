# Publicis Sapient

## Round 1 (project)

You have to develop one microservice using API service.(consume the service from API and expose). Use design principles, patterns, write clean code.
Write 2-3 test cases for your codes. Use Draw.io for representing the architecture.
Build Jenkins pipelines. Create docker image.
You need to install some set up (like Jenkins, docker) in your local system for completing the assignment


### Weather Prediction
```
Problem Statement (Full Stack – UI, Service + CI/CD)

Develop, test and deploy a micro service to show the output of a city&#39;s (to be taken as an input parameter) next 3 days high and low temperatures. If rain is predicted in next 3 days or temperature goes above 40 degree Celsius then mention &#39;Carry umbrella&#39; or &#39;Use sunscreen lotion&#39; respectively in the output, for that day; Demonstrate adding additional conditions, with the least code changes &amp; deployment:

1. In case of high winds (i.e.,) Wind &gt; 10mph, mention “It’s too windy, watch out!”
2. In case of Thunderstorms, mention “Don’t step out! A Storm is brewing!”
3. End user should be able to view results by changing the input parameters
• The service should be ready to be released to production or live environment
• The service should be accessible via web browser or postman (using any one of

JavaScript frameworks, HTML or JSON)
• The solution should support offline mode with toggles
• The service should return relevant results as expected, even while the underlying
dependencies (Ex: Public API) are not available!
(Use your own code/logic/data structures and without 3rd party libraries or DB)
API Data Sources
APIs
https://api.openweathermap.org/data/2.5/forecast?q=london&amp;appid=d2929e9483efc82c
82c32ee7e02d563e&amp;cnt=10
Key: d2929e9483efc82c82c32ee7e02d563e
Documentation: https://openweathermap.org/api
Note: Please use the above API end-point only; The API Key might not work for other
APIs in the documentation
Expected output
(via an UI mechanism of your choice – Ex: React page)
1. List of temperatures along with date
2. Prediction along with the time window
NFRs
• Demonstrate SOLID, 12 Factor and HATEOAS principles, Design Patterns in the
design and implementation
• Demonstrate Performance, Optimization &amp; Security aspects
• Demonstrate Production readiness of the code
• Demonstrate TDD &amp; BDD &amp; Quality aspects
• Demonstrate sensitive information used in the Micro Services such as API keys are
protected / encrypted

Documentation
• Include the open-API spec./Swagger to be part of the code. Should be able to view
API via swagger (Documentation to explain the purpose of the API along with Error
codes that the service consumers &amp; client must be aware of!)
• Create a README.md file in the repository and explain the design and implementation
approach
• In the README, add a sequence diagram or flowchart created using draw.io –
https://www.draw.io
• Mention the design patterns used in the code
Build &amp; Deploy
CI
• Build CI/CD pipeline for your project(s); Pipeline scripts need to be part of the
codebase;
• Ensure the Jenkins job config., scripts are a part of the project sources
CD
• Demonstrate the service deployment using a Docker container (Create a docker image
and publish service locally)
• Ensure the docker files are a part of the project sources
Instructions reg. IDE
• Only 8080 port is available on preview panel. Configure your application on 8080 port
only.
```
