# **Python Project Template**

A flexible and reusable Cookiecutter template to kickstart your Python projects with best practices, pre-configured tools, and a modular structure. Perfect for building apps, APIs, or utilities without starting from scratch every time.

---

## **Features**
- **Modular Structure**: Organized folders and files for clean, maintainable projects.
- **Pre-Configured Logging**: Includes rotating file handlers and colorful console output using `colorlog`.
- **Environment Management**: Supports `.env` files with `python-dotenv`.
- **Versioning System**: Easy version bumping with `bump-my-version`.
- **Cookiecutter Customization**: Dynamically set project name, author, version, and more during initialization.

---

## **Usage**

### 1. Install Cookiecutter
Ensure you have Cookiecutter installed. If not, install it using pip:
```bash
pip install cookiecutter
```

### 2. Generate a New Project
Run Cookiecutter and point it to your template repository:
```bash
cookiecutter https://github.com/<your-username>/python-project-template
```

### 3. Fill Out Prompts
Cookiecutter will ask for details to personalize your project. Example prompts:
- **`project_name`**: The name of your project (e.g., `awesome_project`).
- **`author_name`**: Your name (e.g., `Jake Peralta`).
- **`version`**: The starting version (e.g., `0.1.0-alpha`).
- **`description`**: A short description of your project.

### 4. Explore Your New Project
After running Cookiecutter, your new project will be ready to go:
awesome_project/
│
├── PROJECT_NAME/
│   ├── __init__.py
│   ├── version.py
│   └── utils/
│       ├── logger.py
│       └── ...
├── requirements.txt
├── README.md
├── .gitignore
├── LICENSE

## **Included Tools**

### Logging
Pre-configured logging with:
- Rotating file handlers.
- Colorful console logs (via `colorlog`).
- Easy toggling between console and file logs.

### Environment Variables
Supports `.env` files for managing secrets like API keys. Simply create a `.env` file:
```env
OPENAI_API_KEY=your-api-key
```

### Versioning
Easily bump versions using `bump-my-version`. Example:

``` bash
bump-my-version bump prerelease
bump-my-version release
```

## **Requirements**

### Python Libraries
Make sure the following libraries are installed:
- `colorlog`
- `python-dotenv`
- `bump-my-version`

Install them with:
```bash
pip install -r requirements.txt
```

## **License**
This template is licensed under the MIT License. Feel free to use it, modify it, and distribute it as you wish.
