# 🛠️ ollama-engineer

Originally forked from [o1-engineer](https://github.com/Doriandarko/o1-engineer)

![Updated Features](https://img.shields.io/badge/Features-Updated-brightgreen)

A command-line tool designed to assist developers in managing and interacting with their projects efficiently. Leveraging the power of Ollama's local language models, ollama-engineer provides functionalities such as code generation, file editing, project planning, and code review to streamline your development workflow.

## 🛠️ Updated Features

- **Local LLM Integration**: Now uses Ollama for local language model processing, eliminating the need for an external API.
- **Model Selection**: Users can choose from available Ollama models at startup.
- **Enhanced File and Folder Management**: The `/add` and `/edit` commands support adding and modifying both files and folders, providing greater flexibility in managing your project structure.
- **Project Planning**: The `/planning` command allows users to create comprehensive project plans that can be used to generate files and directories systematically.
- **Advanced Workflows**: New examples demonstrate how to integrate planning and creation commands for efficient project setup.

## ✨ Features

- **Automated Code Generation**: Generate code for your projects effortlessly using local LLMs.
- **File Management**: Add, edit, and manage project files directly from the command line.
- **Interactive Console**: User-friendly interface with rich text support for enhanced readability.
- **Conversation History**: Save and reset conversation histories as needed.
- **Code Review**: Analyze and review code files for quality and suggestions.
- **Project Planning**: Create comprehensive project plans to guide development.

## 💡 How the Script Works

1. **Initialization**: The script initializes global variables and sets up the connection to Ollama.
2. **Model Selection**: Users choose from available Ollama models at startup.
3. **Handling User Commands**: It listens for user commands such as `/edit`, `/create`, `/add`, `/review`, and `/planning`, processing them accordingly.
4. **Processing File and Folder Modifications**: Based on the user's instructions, the script modifies files and folders, adds new content, or creates new files and folders as needed.
5. **AI-Generated Instructions**: The tool interacts with Ollama to generate instructions and suggestions for code generation, editing, project planning, and reviewing.
6. **Applying Changes**: Changes are applied to the project files and folders based on the AI-generated instructions.
7. **Managing Conversation History and Added Files**: The script manages the conversation history and keeps track of files and folders added to the context.

## 📥 Installation

### Prerequisites

- **Python**: Ensure you have Python 3.7 or higher installed. [Download Python](https://www.python.org/downloads/)
- **Ollama**: Install Ollama on your system. [Ollama Installation Guide](https://github.com/ollama/ollama)

### 🔧 Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/ollama-engineer.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd ollama-engineer
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## 📚 Usage

Launch the application using the following command:
```bash
python ollama-eng.py
```

### 🎮 Available Commands

- `/edit`: Edit files or folders (followed by file or folder paths)
- `/create`: Create files or folders (followed by instructions)
- `/add`: Add files or folders to context (followed by file or folder paths)
- `/planning`: Plan project structure and tasks (followed by instructions)
- `/debug`: Print the last AI response
- `/reset`: Reset chat context and clear added files
- `/review`: Review and analyze code files for quality and potential improvements (followed by file or folder paths)
- `/quit`: Exit the program

### 🚀 Advanced Workflows

Here's an example workflow that demonstrates using `/planning` followed by `/create` to generate files based on the created plan:

1. **Planning the Project**:
   ```
   You: /planning Create a basic web application with the following structure:
   - A frontend folder containing HTML, CSS, and JavaScript files.
   - A backend folder with server-side scripts.
   - A README.md file with project documentation.
   ```

2. **Creating the Project Structure based on the Plan**:
   ```
   You: /create Generate the project structure based on the above plan.
   ```

This demonstrates how to use the new `/planning` command to define a project structure, and then `/create` to generate the files and folders accordingly.

### 📝 Examples

```bash
You: /add src/main.py src/utils/helper.py src/models/

You: /planning Outline a RESTful API project with separate folders for models, views, and controllers.

You: /create Set up the basic structure for a RESTful API project with models, views, and controllers folders, including initial files.

You: /edit src/main.py src/models/user.py src/views/user_view.py
```

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.

2. Create a new branch (`git checkout -b feature/YourFeature`).

3. Commit your changes (`git commit -m 'Add some feature'`).

4. Push to the branch (`git push origin feature/YourFeature`).

5. Open a pull request.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=ZacharyZhang-NY/Ollama-Engineer&type=Date)](https://github.com/ZacharyZhang-NY/Ollama-Engineer&Date)

