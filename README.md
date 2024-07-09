<!-- # Penwise Journalling App

<div align="center">

```bash
    This React Native Expo app enables user authentication for signup and login, 
    facilitates management of journal entries including creation, editing, 
    and deletion with categorization options (e.g., Personal, Work, Travel),
    The app also offers a summary view of entries by selected periods, categories
    and allows users to update their username and password settings.
```
</div>

## Table of Contents

- [Prerequisites](#prerequisites)
- [App Installation and Running in Development Mode](#app-installation-and-running-in-development-mode)
- [Building the Application](#building-the-application)
- [Tests](#tests)
- [Project Directory Structure](#project-directory-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)



## Prerequisites

Before setting up the project, ensure you have the following installed.
These are necessary for installing dependencies and running scripts specified
in the `package.json` for the React Native Expo app.

| Binaries      | Version    |
| ------------- | ---------- |
| Node.js       | >= 18.9.1  |
| npm           | >= 9.2.0   |
| Expo CLI      | >= 6.3.10  |
| TypeScript    | >= 4.0.0   |


## App Installation and Running in Development Mode

1. Clone the repository:

```sh
    git clone https://github.com/james-mumo/PenWise-Journaling-App.git
```

2. Navigate to the project directory:

```sh
    cd frontend
```

3. Setup Env Variables:

```sh
    # create a .env file and add the following variable:
    BASE_URL = <backend_url>
```

4. Install dependencies:

```sh
    npm install
```


5. Run the app in development mode:

```sh
    # Start the Expo Development Server 
    npx expo start

    # Ensure your Android device is connected via USB debugging
    npx expo start --android

    # Ensure your iOS device is connected via USB or open in simulator
    npx expo start --ios

    # To run on a device with the Expo-Go app ensure the device running
    # Expo-Go app is in the same network as your machine, then scan the qr code and hit {r} to refresh whenever you make changes.

```

## Building the Application

```bash

    # For building an Android APK:
    npx expo build:android

    # For building an iOS IPA file:
    npx expo build:ios

```


## Tests 

```bash

```




## Project Directory Structure

```bash
/frontend
├── app
│   ├── (auth)
│   │   ├── html.tsx
│   │   ├── _layout.tsx
│   │   └── search
│   ├── (tabs)
│   │   ├── not-found.jsx
│   │   └── index.tsx
│   └── index.tsx
├── assets
│   ├── adaptive-icon.png
│   ├── fonts
│   ├── icons
│   ├── splash.png
│   ├── favicon.png
│   └── icon.png
├── components
│   ├── AddCategoryModal.jsx
│   ├── CategoryCard.jsx
│   ├── CustomButton.jsx
│   ├── EmptyState.jsx
│   ├── FormContentField.jsx
│   ├── FormField.jsx
│   ├── InfoBox.jsx
│   ├── JournalEntryCard.jsx
│   ├── JournalEntryModal.jsx
│   ├── Loader.jsx
│   ├── SearchInput.jsx
│   └── index.js
├── constants
│   ├── icons.js
│   ├── images.js
│   └── index.js
├── context
│   └── GlobalProvider.js
├── hooks
│   ├── useCategories.jsx
│   ├── useColorScheme.web.ts
│   ├── useColorScheme.ts
│   ├── useDateTime.jsx
│   ├── useDateFormatter.ts
│   └── useThemeColor.ts
├── lib
│   ├── appwrite.js
│   └── useAppwrite.js
└── scripts
    └── reset-project.js
├── README.md
├── babel.config.js
├── expo-env.d.ts
├── tailwind.config.js
├── app.json
├── package-lock.json
├── tsconfig.json
├── twindConfig.js
├── package.json


```

## Technologies Used

```bash
    - Expo
    - @react-native-async-storage/async-storage
    - @react-native-community/datetimepicker
    - @react-native-picker/picker
    - @react-navigation/bottom-tabs
    - @react-navigation/native
    - axios
    - expo-document-picker
    - expo-linking
    - nativewind
    - react-native-animatable
    - react-native-appwrite
    - react-native-reanimated
    - react-navigation
    - @types/jest
    - tailwindcss
    - typescript
```

## Contributing

## License -->

## Express, Typescript with Postgres Backend

<div align="center">

```bash
    This is the backend service for the React-Native Frontend 
    built with Express.Js, Typescript and Postgres DB
```

</div>


## Prerequisites

Before running and intsalling the project's backend service, ensure you have the following installed.

| Binaries      | Version    |
| ------------- | ---------- |
| Node.js       | >= 18.9.1  |
| npm           | >= 9.2.0   |
| TypeScript    | >= 4.0.0   |
| Ngrok         | >= 3.8.0  |



## Backend Setup & Installation

1. Clone the repository:

```bash

    git clone https://github.com/james-mumo/PenWise-Journaling-App

    cd backend
```

2. Install dependencies:

```bash
    npm install
```

3. Configure Environment Variables:

    -   In the root directory of your project, create a file named .env & add the following variables:

```bash
    # Backend server port
    PORT=""

    # (can be generated securely using crypto.randomBytes(64).toString('hex'))
    JWT_ACCESS_SECRET=""
    JWT_REFRESH_SECRET=""


    # PostgreSQL connection URL
    DATABASE_URL=postgres://postgres:123456@localhost:5432/penwise

```


3. Migration and Database Initialization

```bash 
    - Run the SQL script named {init.sql} to initialize the schema and seed any default data you might need

    - Ensure the PostgreSQL service is up and running.

```


## Application Availability

```bash
    The application will be available at http://localhost:${PORT}.
```


## Contribution
        ```bash
        Feel free to submit issues, fork the repository, and send pull requests!
        This project is a take-home assignment that I am working on independently.
        However, if you are interested in the application, you are welcome to fork
        the repository and contribute to making it better as per your wish.
        ```




## Project Directory Structure

The backend project is organized into several folders and files, each serving a specific purpose. Below is the file tree representation of the project:

```bash

backend/
├── config/
│   └── database.ts
├── controllers/
│   ├── authController.ts
│   ├── categoryController.ts
│   └── journalEntryController.ts
├── dist/
│   ├── config/
│   ├── controllers/
│   ├── index.js
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── types/
│   └── utils/
├── middlewares/
│   └── authMiddleware.ts
├── models/
│   ├── Category.ts
│   ├── JournalEntry.ts
│   └── User.ts
├── routes/
│   ├── auth.ts
│   ├── categoryRoutes.ts
│   └── journalEntryRoutes.ts
│── types/
│    └── index.ts
├── README.md
├── index.ts
├── package-lock.json
├── tsconfig.json
├── env.example
├── init.sql
└── package.json


```


## Folder and File Descriptions

- **config**: Contains configuration files.
  - `database.ts`: Database connection and configuration.

- **controllers**: Contains the controller files that handle the application logic for different routes.
  - `authController.ts`: Handles user authentication-related operations.
  - `journalEntryController.ts`: Manages journal entries.

- **dist**: Compiled output directory.
  - `ex.ts`: Example or test file.
  - `index.ts`: Entry point of the application.

- **init.sql**: SQL initialization script for setting up the database schema.

- **middlewares**: Contains middleware files.
  - `authMiddleware.ts`: Middleware for authentication.

- **models**: Contains the data models.
  - `JournalEntry.ts`: Model for journal entries.
  - `User.ts`: Model for users.

- **routes**: Contains the route files.
  - `auth.ts`: Routes for user authentication.
  - `journalEntryRoutes.ts`: Routes for journal entry operations.

- **tsconfig.json**: TypeScript configuration file.

- **utils**: Utility functions.
  - `jwt.ts`: Functions for handling JSON Web Tokens (JWT).

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (version >= 16.0.0)
- PostgreSQL (version >= 9.0)

### Dependencies

```json
"dependencies": {
  "bcrypt": "^5.1.1",
  "dotenv": "^16.4.5",
  "express": "^4.19.2",
  "jsonwebtoken": "^9.0.2",
  "pg": "^8.12.0"
}
```

```json
"devDependencies": {
  "@types/bcrypt": "^5.0.2",
  "@types/dotenv": "^8.2.0",
  "@types/express": "^4.17.21",
  "@types/jsonwebtoken": "^9.0.6",
  "@types/pg": "^8.11.6",
  "nodemon": "^3.1.4",
  "typescript": "^5.5.3"
}
```
