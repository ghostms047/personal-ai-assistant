# Personal AI Assistant

An Android personal AI assistant designed to work as the device's default assistant while using an external AI API for intelligent responses and actions.

## Features

- External AI API integration
- API key configuration from Settings
- Text and voice interaction
- Screen understanding when the required Android permissions are granted
- Launch and inspect installed apps
- Search and open accessible files
- Local file indexing for fast natural-language search
- Floating assistant overlay
- Android default assistant integration
- Permission-aware actions using official Android APIs
- Background and incremental indexing
- Modern, clean, minimal UI

## Architecture

The assistant follows a tool-based architecture:

**User → AI → Tool/Action → Permission Check → Android API → Result → AI → User**

Example actions include:

- Open an app
- Search installed apps
- Get app information
- Search files
- Open files
- Inspect the current screen
- Read visible screen text
- Summarize the current screen
- Create or update the file index
- Open Android settings
- Ask the user for clarification

## Android & Security

The project is intended to use official Android APIs and permission models, including:

- Android Assistant APIs
- Accessibility APIs where appropriate
- Storage Access Framework (SAF)
- MediaStore
- Android screen-capture APIs where appropriate
- Room / SQLite for local indexing

The app does **not** rely on arbitrary shell commands or security bypasses.

## API Key

The AI provider and API key are configured by the user from the app's Settings screen.

> Never commit a real API key, token, password, or other secret to this repository.

## Tech Stack

- Kotlin
- Jetpack Compose
- MVVM / Clean Architecture
- Coroutines
- StateFlow
- Room / SQLite
- WorkManager
- Android SDK

## Project Status

🚧 **In development**

The project focuses on reliability, privacy, performance, and a polished Android user experience.

## License

This project does not currently specify a license.
