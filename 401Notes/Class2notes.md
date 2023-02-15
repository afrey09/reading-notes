Express, NPM, TDD, CI/CD

An introduction to NodeJS and Express

Explain middleware, answer as though I were a non-technical recruiter.
  Software that acts as the middleman between the os or database and applications

Express the most popular - Node web framework

Express is “unopinionated.” What does that mean?
  "Express is unopinionated. You can insert almost any compatible middleware you like into the request handling chain, in almost any order you like. You can structure the app in one file or multiple files, and using any directory structure."

What is a module and why is modularity useful to us as developers?
  "A module is a JavaScript library/file that you can import into other code using Node's require() function". It is useful for helping keep your code more organized and therefore easier to debug.

What is NPM?

What version of npm are you running on your machine? 9.4.0
What command would you type to install a library/package called ‘jshint’ into your node project? npm i jshint

What is TDD?

Explain why tests are important. Please explain as though I were your non technical elder.
  Testing is important because it allows us to ensure that applications we create work properly and are free of errors.

What are three expected benefits of testing

  - signifcant reductions in defect rates
  - reduction in effort in projects' final phases
  - improvied design qualities in the code

Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.

  - forgetting to run tests frequently
  - writing too many tests at once

  Team..
  - partial adoption – only a few developers on the team use TDD
  - poor maintenance of the test suite – most commonly leading to a test suite with a prohibitively long running time

CI/CD

What are three benefits of Continuous Integration? "Ensures everyone's changes integrate, catch bugs and reduce merge conflicts"

What is the difference between Continuos Delivery and Continuous Deployment?
Cont. Delivery "the practice of developing software in such a way that you can release it at any time."
Cont. Deployment " An extension of Cont. Delivery but deploys new features immediately."

Explain how GitHub fits into this process assuming the listener comes from a non-technical background
  Devs make changes locally and push to github when they want to share it with others. Github uses webhooks to then send messages to external servers and then runs tests on received info to see which changes can be integrated into the main branch."

Sources:
https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction
https://docs.npmjs.com/about-npm/
https://www.agilealliance.org/glossary/tdd/
https://www.youtube.com/watch?v=xSv_m3KhUO8
