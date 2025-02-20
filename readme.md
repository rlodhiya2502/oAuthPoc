# OAuth Proof of Concept

This project demonstrates how to implement Google and Apple Single Sign-On (SSO) using HTML5, CSS3, and JavaScript without any third-party dependencies. It also includes the use of localStorage, IndexedDB, and encryption/decryption for sensitive information. The server-side is implemented using NestJS.

## Table of Contents
- [OAuth Proof of Concept](#oauth-proof-of-concept)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Features](#features)
  - [Requirements](#requirements)
  - [Setup](#setup)
  - [Usage](#usage)
  - [License](#license)

## Introduction
This proof of concept (PoC) showcases the implementation of Google and Apple SSO. The goal is to provide a simple and secure way for users to authenticate using their Google or Apple accounts. Additionally, it demonstrates the use of localStorage, IndexedDB, and encryption/decryption for handling sensitive information.

## Features
- Google Single Sign-On
- Apple Single Sign-On
- Pure HTML5, CSS3, and JavaScript
- No third-party dependencies
- Utilization of localStorage and IndexedDB
- Encryption and decryption of sensitive information
- Fullstack application with NestJS for server-side

## Requirements
- A web browser (latest version recommended)
- Google Developer account
- Apple Developer account
- Node.js and npm (for server-side)
- NestJS framework

## Setup
1. **Clone the repository:**
        ```sh
        git clone https://github.com/yourusername/oAuthPoc.git
        cd oAuthPoc
        ```

2. **Google SSO Setup:**
        - Go to the [Google Developer Console](https://console.developers.google.com/).
        - Create a new project.
        - Enable the "Google+ API" for the project.
        - Create OAuth 2.0 credentials and set the authorized JavaScript origins and redirect URIs.

3. **Apple SSO Setup:**
        - Go to the [Apple Developer Account](https://developer.apple.com/account/).
        - Create a new App ID.
        - Configure the Sign In with Apple service.
        - Generate a private key for authentication.

4. **Configure the project:**
        - Update the `config.js` file with your Google and Apple credentials.

5. **Server-side Setup:**
        - Install dependencies:
            ```sh
            npm install
            ```
        - Start the NestJS server:
            ```sh
            npm run start
            ```

## Usage
1. Open `index.html` in your web browser.
2. Click on the "Sign in with Google" or "Sign in with Apple" button.
3. Follow the authentication flow to sign in.
4. Sensitive information will be stored securely using localStorage and IndexedDB with encryption.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.