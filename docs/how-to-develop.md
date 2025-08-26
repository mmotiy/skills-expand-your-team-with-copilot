# Development Guide

## For Teachers: Requesting Changes

If you're a teacher looking to request changes to the activity management system, please use our structured issue templates instead of modifying code directly:

**[📝 Create a New Request](https://github.com/mmotiy/skills-expand-your-team-with-copilot/issues/new/choose)**

Available templates:
- 🎯 **Add New Activity** - For creating new clubs, sports, or activities
- ✏️ **Modify Existing Activity** - For changing schedules, capacity, or details
- 🎨 **UI/UX Improvement** - For interface enhancements
- 🐛 **Bug Report** - For reporting problems or errors
- ✨ **New Feature Request** - For requesting new capabilities
- 📊 **Data Management** - For bulk operations or data import/export

[📖 See the full template guide](.github/ISSUE_TEMPLATE/README.md) for detailed help on which template to use.

## For Developers: Initial Setup

This project is best developed using GitHub Codespaces, which provides a consistent development environment with all the necessary tools pre-configured.

### Setting up your development environment

1. Open the repository in a codespace
2. Wait for the container to finish building and installing dependencies
3. Install Python dependencies by running:

   ```bash
   python -m pip install -r requirements.txt
   ```

### Dependencies

The project requires the following Python packages:

- FastAPI - Modern web framework for building APIs
- Uvicorn - ASGI server implementation for running the FastAPI application

These dependencies will be installed when you run `pip install -r requirements.txt`

## Debugging

### Running the website locally

1. From VS Code's Run and Debug view (Ctrl+Shift+D), select "Launch Mergington WebApp" from the launch configuration dropdown
2. Press F5 or click the green play button to start debugging
3. The website will be available at `http://localhost:8000`
4. The API documentation will be available at `http://localhost:8000/docs`

### Debugging tips

- FastAPI's auto-reload feature will automatically restart the server when you make code changes
- Use the interactive API documentation at `/docs` to test your endpoints

## Getting Started

1. Install the dependencies:

   ```bash
   pip install fastapi uvicorn
   ```

2. Run the application:

   ```bash
   python app.py
   ```

3. Open your browser and go to:
   - API documentation: http://localhost:8000/docs
   - Alternative documentation: http://localhost:8000/redoc

## Usage

### API Endpoints

| Method | Endpoint                                                          | Description                                                         |
| ------ | ----------------------------------------------------------------- | ------------------------------------------------------------------- |
| GET    | `/activities`                                                     | Get all activities with their details and current participant count |
| POST   | `/activities/{activity_name}/signup?email=student@mergington.edu` | Sign up for an activity                                             |

> [!IMPORTANT]
> All data is stored in memory, which means data will be reset when the server restarts.
