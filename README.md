# Angular Redux Animal Kingdom

An animal management system where users can browse, add, and manage animals. Features user authentication, animal listings, and statistics dashboard.

## Tech Stack

### Frontend
| Category | Technology |
|----------|------------|
| Framework | Angular 4 |
| State Management | @angular-redux/store |
| UI Components | Angular Material |
| Language | TypeScript |
| Build Tool | Angular CLI |

### Backend
| Category | Technology |
|----------|------------|
| Runtime | Node.js |
| Framework | Express.js |
| Authentication | Passport.js, JWT |
| Validation | Validator.js |

## Features

- **User Authentication** - Register and login with JWT tokens
- **Animal Listings** - Browse and view animal details
- **Add Animals** - Create new animal entries
- **Statistics** - View animal statistics dashboard
- **Material Design** - Clean UI with Angular Material

## Prerequisites

- [Node.js](https://nodejs.org/) (v6 or higher)
- [Angular CLI](https://cli.angular.io/) (`npm install -g @angular/cli`)
- npm or yarn

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/nikolaykolibarov/angular-redux-animal-kingdom.git
   cd angular-redux-animal-kingdom
   ```

2. **Install server dependencies**
   ```bash
   cd server
   npm install
   ```

3. **Install client dependencies**
   ```bash
   cd ../client
   npm install
   ```

## Running the Application

1. **Start the backend server**
   ```bash
   cd server
   npm start
   ```

2. **Start the frontend (in a new terminal)**
   ```bash
   cd client
   ng serve
   ```

3. **Open in browser**
   ```
   http://localhost:4200
   ```

## Project Structure

```
angular-redux-animal-kingdom/
├── client/                     # Angular frontend
│   ├── src/
│   │   └── app/
│   │       ├── account/       # User account components
│   │       ├── animals/       # Animal-related components
│   │       ├── authentication/# Auth components (login, register)
│   │       ├── layouts/       # Layout components
│   │       ├── shared/        # Shared utilities
│   │       ├── store/         # Redux store configuration
│   │       ├── app.module.ts  # Main app module
│   │       └── app-routing.module.ts
│   ├── package.json
│   └── tsconfig.json
│
└── server/                     # Express backend
    ├── data/                  # Data storage
    ├── middleware/            # Express middleware
    ├── passport/              # Passport configuration
    ├── routes/
    │   ├── animals.js         # Animal CRUD routes
    │   ├── auth.js            # Authentication routes
    │   └── stats.js           # Statistics routes
    ├── index.js               # Server entry point
    └── package.json
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/auth/register` | Register new user |
| POST | `/auth/login` | Login user |
| GET | `/animals` | Get all animals |
| POST | `/animals` | Create new animal |
| GET | `/stats` | Get statistics |

## License

MIT

---

> **Note:** This project was created as an exam solution for the Angular 2 Fundamentals course at Software University. It is intended for local viewing and demonstration purposes only.
