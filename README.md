# Aurelyn.Admin

## Hospital Healthcare Management System — Admin Portal

Aurelyn.Admin is the Angular-based administrative frontend for the Aurelyn Hospital Healthcare Management System. It provides a centralized interface for hospital administrators to manage hospital operations, users, staff, patient information, appointments, and role-based access.

## Overview

The application is designed to provide a responsive, intuitive, and secure administrative experience. It communicates with Aurelyn.Api to retrieve and manage data while enforcing access based on user roles and permissions.

## Key Features

- **Admin Dashboard** — Centralized overview of hospital operations.
- **Patient Management** — Access and manage patient information according to permissions.
- **Staff Management** — Manage hospital staff and user accounts.
- **Appointment Management** — View and manage appointment workflows.
- **Role-Based Access Control** — Display authorized features based on user roles.
- **User Management** — Support administrative account management.
- **API Integration** — Communicate with Aurelyn.Api for backend operations.
- **Responsive UI** — Provide a consistent experience across supported devices.

*Features should be updated to reflect the functionality implemented in the application.*

## Technology Stack

- **Frontend Framework:** Angular
- **Language:** TypeScript
- **UI:** HTML and CSS / SCSS
- **API Communication:** Angular HttpClient
- **Backend:** ASP.NET Core Web API (`Aurelyn.Api`)
- **Version Control:** Git and GitHub

## Project Structure

```text
Aurelyn.Admin/
├── src/
│   ├── app/
│   │   ├── core/
│   │   ├── shared/
│   │   ├── features/
│   │   ├── services/
│   │   └── app.routes.ts
│   ├── assets/
│   ├── environments/
│   ├── index.html
│   └── styles.scss
├── angular.json
├── package.json
├── tsconfig.json
└── README.md
```

*This is a suggested structure. Adjust it to match your actual Angular project.*

## Getting Started

### Prerequisites

Install the following tools:

- Node.js compatible with your Angular version
- npm
- Angular CLI
- Visual Studio Code or another supported editor
- Git

### Clone the Repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd Aurelyn.Admin
```

### Install Dependencies

```bash
npm install
```

### Configure the API

Configure the backend API base URL in the appropriate Angular environment or application configuration file.

Ensure that Aurelyn.Api is running and that the frontend is configured to communicate with the correct development endpoint.

Do not commit credentials, API secrets, or production environment settings to source control.

### Run the Application

```bash
ng serve
```

Open the local URL displayed in the terminal, typically:

`http://localhost:4200/`

### Build for Production

```bash
ng build
```

The generated build output will be placed in the configured output directory.

## Security

- Integrate with the authentication mechanism provided by Aurelyn.Api.
- Apply route guards for frontend navigation and user experience.
- Enforce authorization on the backend; frontend guards alone are not security controls.
- Avoid storing sensitive patient information in browser storage unnecessarily.
- Use HTTPS in appropriate environments.
- Never commit secrets or real patient data.

## Branching Strategy

- `master` — Protected branch for stable code.
- `feature/*` — New frontend features.
- `bugfix/*` — Bug fixes.
- `hotfix/*` — Urgent fixes.

Submit changes through pull requests and review them before merging into the protected branch.

## Development Guidelines

1. Follow Angular and TypeScript coding conventions.
2. Use reusable components and shared services.
3. Keep API communication in appropriate services.
4. Use lazy loading where suitable.
5. Maintain consistent error handling and form validation.
6. Test important components, services, and user workflows.
7. Keep dependencies updated and compatible with the project's Angular version.

## License

Specify the applicable license before distributing or making this project available for reuse.

---

**Aurelyn.Admin** — Administrative frontend for the Aurelyn Hospital Healthcare Management System.
