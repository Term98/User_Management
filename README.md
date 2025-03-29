# User Management Application

A React application that integrates with the Reqres API to perform basic user management functions. Built with React, TypeScript, and Tailwind CSS.

## Features

- User Authentication
- User List with Pagination
- Edit User Details
- Delete Users
- Protected Routes
- Responsive Design

## Prerequisites

- Node.js (v16 or higher)
- npm (v7 or higher)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd user-management-app
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5173`

## Usage

### Authentication

- Use the following credentials to log in:
  - Email: eve.holt@reqres.in
  - Password: cityslicka

### User Management

- View Users: Navigate to the users list page after login
- Edit User: Click the edit icon next to a user
- Delete User: Click the delete icon next to a user
- Pagination: Use the page numbers at the bottom to navigate through users

## Project Structure

```
src/
├── components/     # Reusable components
├── pages/         # Page components
├── services/      # API services
├── types/         # TypeScript types
└── main.tsx       # Application entry point
```

## Technical Stack

- React 18
- TypeScript
- Tailwind CSS
- React Router DOM
- Axios
- Lucide React (for icons)
- React Hot Toast (for notifications)

## API Integration

The application integrates with the Reqres API (https://reqres.in/) for:
- User authentication
- Fetching user data
- Updating user information
- Deleting users

## Development

- Run development server: `npm run dev`
- Build for production: `npm run build`
- Preview production build: `npm run preview`

## Notes and Considerations

1. Token Management
   - Authentication token is stored in localStorage
   - Protected routes redirect to login if no token is present

2. Error Handling
   - API errors are caught and displayed using toast notifications
   - Form validation is implemented for all input fields

3. State Management
   - React's built-in useState and useEffect hooks are used for state management
   - Props are used for component communication

4. Security
   - Protected routes implementation
   - Token-based authentication
   - API error handling