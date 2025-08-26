# Mergington High School Activities

A comprehensive web application for managing extracurricular activities at Mergington High School. The system allows teachers to register students for activities while providing advanced search and filtering capabilities for browsing available programs.

## Features

### For Teachers
- **Secure Authentication**: Login with username and password to access management features
- **Student Registration**: Register students for activities using their email addresses
- **Student Management**: Unregister students from activities when needed
- **Session Management**: Persistent login sessions with automatic validation

### For Everyone
- **Activity Browsing**: View all available extracurricular activities with detailed information
- **Advanced Search**: Search activities by name, description, or schedule details
- **Smart Filtering**: Filter activities by multiple criteria:
  - **Category**: Sports, Arts, Academic, Community, Technology
  - **Day of Week**: Monday through Sunday, including weekends
  - **Time Range**: Before School, After School, Weekend activities
- **Detailed Information**: View schedules, participant counts, maximum capacity, and descriptions
- **Responsive Design**: Modern, mobile-friendly interface with intuitive navigation

### System Features
- **Real-time Updates**: Live participant counts and availability status
- **Data Persistence**: MongoDB database storage for activities and user data
- **RESTful API**: FastAPI backend with comprehensive endpoint documentation
- **Modern Frontend**: Interactive JavaScript interface with modal dialogs and dynamic filtering

## Technology Stack

- **Backend**: FastAPI (Python) with RESTful API design
- **Database**: MongoDB for persistent data storage
- **Frontend**: Vanilla JavaScript with modern ES6+ features
- **Authentication**: Secure password hashing with session management
- **Styling**: CSS with responsive design principles

## User Roles

- **Teachers**: Can log in to register/unregister students for activities
- **Students/Public**: Can browse and search activities (registration requires teacher assistance)

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).
