### Conceptual Exercise

Answer the following questions below:

- What is a JWT?  

  A JSON web token, used to store info and authenticate a user when signing in on required sites.

- What is the signature portion of the JWT?  What does it do?  

  The signature portion in the structure of a JWT is the last part. It's the part that can't be decoded and proves that the person with the token is who they say they are.

- If a JWT is intercepted, can the attacker see what's inside the payload?  

  Yes, the payload can be decoded.

- How can you implement authentication with a JWT?  Describe how it works at a high level.  

  First, a token is created and haashed. This token then must be present with each request when attempting to sign in or login, then stored in browser. For each request, the token is sent from browser to server and validated.

- Compare and contrast unit, integration, and end-to-end tests.  

  These tests fall into a spectrum based on scope. Unit tests isolate and verify individual functions. Integration tests focus on how multiple functions interact within a module. End-to-end tests simulate the entire user journey, encompassing the entire application. All involve writing test functions that instruct the app to perform actions and then check the results against expectations.

- What is a mock? What are some things you would mock?  

  Mocks are stand-in objects used in testing to replace complex dependencies that might be difficult to interact with directly during tests. A common example is mocking an external API call to avoid making actual network requests during testing.

- What is continuous integration? 
 
  Continuous integration is a practice of automating code building, testing, and deployment in frequent, incremental cycles. This allows for early detection of bugs and ensures a smooth development flow.

- What is an environment variable and what are they used for?  

  Environment variables are a way to store configuration data that can influence the entire application. A typical use case involves setting a variable to indicate whether the app is in a testing environment, which might influence the database connection used.

- What is TDD? What are some benefits and drawbacks?  

  TDD is a development approach where writing tests precedes actual code implementation. While it can initially slow down coding, it can lead to faster overall development by directing code with clear expectations and preventing unnecessary tangents. However, TDD can have a steeper learning curve for those unfamiliar with the methodology.

- What is the value of using JSONSchema for validation? 
 
  JSONSchema provides a way to define the expected structure and format of JSON data. This can save significant time writing validation code, especially when multiple functions interact with the same data structures.

- What are some ways to decide which code to test?  

  Here are some factors to consider when deciding which code to test:

  - Importance: Prioritize testing for critical application functionalities.
  - Testability: Functions that are easier to isolate and test can be prioritized for earlier coverage.
  - Edge Cases: Include tests that cover unusual or boundary conditions to ensure robustness.

- What are some differences between Web Sockets and HTTP?
  
  Both protocols facilitate communication between clients and servers. However, HTTP operates on a request-response model, meaning the client sends a request and receives a response before initiating a new interaction. WebSockets, on the other hand, establish a persistent, two-way connection, allowing for real-time data exchange as changes occur.

- Did you prefer using Flask over Express? Why or why not? 
  This is subjective, and both frameworks have their merits. I prefer Flask due to its perceived tendency to promote cleaner and more concise Python code, compared to more verbose JavaScript code in Express. Additionally, the "try/catch" approach in Express feels less efficient than potential Python/Flask alternatives.
