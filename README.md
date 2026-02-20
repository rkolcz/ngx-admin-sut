### ngx-admin-sut

System Under Test (SUT) application based on the open-source **ngx-admin** Angular dashboard template.

This repository contains a frontend application used as a System Under Test (SUT) for Playwright automation testing.

The application itself is not the purpose of this project. It exists only to provide a real UI for automated UI, E2E and visual regression tests.

The automated tests are located in a separate repository.

The original project was created by the Akveo Team:
https://github.com/akveo/ngx-admin

The original MIT license is preserved in accordance with open-source requirements.
___

### About the project

The application is based on ngx-admin Angular dashboard.

Important:

This is legacy code and is no longer actively maintained.
Modern Node.js environments cannot run it reliably without containerization.

Typical issues without Docker:

dependency conflicts

node-sass build failures

Angular CLI incompatibilities

different rendering across operating systems

Because Playwright visual tests compare pixels, the application must run in a stable and repeatable environment.

For this reason the application is executed inside **Docker**.

___

### Requirements

- Docker 

### Running the application

Running the application

Clone the repository:

```git clone <repo-url>```

Build and start the application:

```docker compose up --build```

### Access the application

After successful startup you should see:

```Angular Live Development Server is listening on 0.0.0.0:4200 Compiled successfully.```

Open browser:

```http://localhost:4200```

### Stop the application

Press:
```CTRL + C```
Then run:
```docker compose down```

### Related repository

Playwright tests:
```in progress```