
# Spotify API Experiment

Welcome to the Spotify API Experiment project! This repository contains the code and documentation for experimenting with the Spotify API using Next.js and NextAuth. This project is a personal endeavor to deepen my understanding of the Spotify API and how to integrate it with modern web technologies. It's designed for developers interested in exploring the capabilities of the Spotify API and learning more about how to work with it in a real-world application.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Demo](#demo)
- [Project Structure](#project-structure)
- [Environment Variables](#environment-variables)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

## Introduction

This project replicates the core functionalities of Spotify, allowing users to log in with their Spotify accounts, browse playlists, search for music, and play songs. The app leverages Next.js for the frontend and backend, NextAuth for authentication, and the Spotify API to fetch and display user-specific data.

## Features

- **User Authentication**: Login with Spotify using NextAuth.
- **Persisted Login Session**: Users stay logged in even after refreshing the page.
- **Spotify API Integration**: Fetch user playlists, songs, and search for music.
- **Responsive UI**: Built with Tailwind CSS, ensuring a seamless experience across devices.
- **Dynamic Routing**: Explore artists, albums, and songs through dynamic routes.
- **Middleware**: Secures the application and manages user sessions.

## Technologies Used

- **Next.js**: React framework for server-side rendering and static site generation.
- **NextAuth**: Authentication for Next.js applications.
- **Spotify API**: Fetching user data and managing playlists.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **Heroicons**: Beautiful hand-crafted SVG icons.
- **JavaScript**: Core programming language.
- **Vercel**: Deployment platform for Next.js applications.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/apoorvnandan/spotify-2-0.git
   ```
2. Navigate to the project directory:
   ```bash
   cd spotify-2-0
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Create a `.env.local` file in the root directory and add your environment variables (see [Environment Variables](#environment-variables) for details).

5. Run the development server:
   ```bash
   npm run dev
   ```

## Usage

Once the development server is running, you can open the app in your browser at `http://localhost:3000`. You will be prompted to log in with your Spotify account, after which you can explore your playlists, search for songs, and enjoy the features of this Spotify clone.

## Demo

### Home Page
![Home Page](./public/s1)

### Playlists Page
![Playlists Page](./public/s2)

### Search Page
![Search Page](./public/s3)

## Project Structure

```
/pages
  - _app.js          # Application wrapper
  - index.js         # Home page
  - login.js         # Login page
  - search.js        # Search page
  - playlists.js     # Playlists page
/components
  - Sidebar.js       # Sidebar component
  - Player.js        # Song player component
/lib
  - spotify.js       # Spotify API helper functions
  - auth.js          # Authentication and token management
```

## Environment Variables

Create a `.env.local` file in the root of your project and add the following variables:

```
NEXTAUTH_URL=http://localhost:3000
NEXT_PUBLIC_SPOTIFY_CLIENT_ID=your_spotify_client_id
NEXT_PUBLIC_SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
NEXT_PUBLIC_JWT_SECRET=your_jwt_secret
```

Ensure you replace `your_spotify_client_id`, `your_spotify_client_secret`, and `your_jwt_secret` with your actual Spotify API credentials and a secret key for JWT.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests.


