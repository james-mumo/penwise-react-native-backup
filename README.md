# Penwise Journalling App

Brief description of your project.

## Table of Contents

- [Introduction](#introduction)
- [Installation Steps](#installation-steps)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Introduction

```bash
    This React Native Expo app enables user authentication for signup and login, facilitates management of journal entries including creation, editing, and deletion with categorization options (e.g., Personal, Work, Travel), offers a summary view of entries by selected periods, and allows users to update their username and password settings
```


### Prerequisites


Before setting up the project, ensure you have the following installed:


| Binaries      | Version    |
| ------------- | ---------- |
| Node.js       | >= LTS     |
| npm           | >= 6.14.6  |
| Expo CLI      | >= 4.0.0   |
| TypeScript    | >= 4.0.0   |
| Tailwind CSS  | >= 3.0.0   |

These are necessary for installing dependencies and running scripts specified in your `package.json` for the React Native Expo app.


### Installation Steps

1. Clone the repository:

git clone <repository_url>

2. Navigate to the project directory:

cd project-directory

3. Install dependencies:

npm install

Instructions on how to use the app. Include any configuration settings if necessary.

### Development

Steps to run the app in development mode.

1. Start the Expo development server:

npm start

2. Follow Expo CLI instructions to run the app on an emulator or physical device.

### Production

Instructions for building and deploying the app for production, if applicable.

## Folder Structure

Explain the structure of your project directory and key files.




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

List of technologies, frameworks, and libraries used in the project.

- React Native
- Expo
- List others...

## Contributing

Guidelines for contributing to the project. Include information on how to submit issues and pull requests.

## License

Specify the project's license. For example:

This project is licensed under the [MIT License](link-to-license-file).
