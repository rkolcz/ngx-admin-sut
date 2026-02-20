### ngx-admin-sut

System Under Test (SUT) application based on the open-source **ngx-admin** Angular dashboard template.

This repository contains a frontend application used as a System Under Test (SUT) for automation testing.

>The application itself is not the purpose of this project. It exists only to provide a real UI for automated UI, E2E and visual regression tests. The automated tests are located in a separate repository.

The original project: https://github.com/akveo/ngx-admin

The original MIT license is preserved in accordance with open-source requirements.
___

### About the project

The application is based on ngx-admin Angular dashboard.

> [!NOTE]
> This is **legacy code** and is no longer actively maintained.
Modern Node.js environments cannot run it reliably without containerization. Typical issues without Docker: dependency conflicts, node-sass build failures or Angular CLI incompatibilities


For this reason the application is executed inside **Docker**.

___

### Requirements

- Docker 

___

### Running the application

1. Clone the repository:

```bash
git clone <repo-url>
```

2. Build and start the application:

```bash
docker compose up --build
```

___

### Access the application

After successful startup you should see:

```bash
Angular Live Development Server is listening on 0.0.0.0:4200
Compiled successfully.
```

Open browser:

```bash
http://localhost:4200
```

___

### Stop the application

Press:

```bash
CTRL + C
```

Then run:

```bash
docker compose down
```

___

### Related repository

Playwright tests:
```bash
in progress
```