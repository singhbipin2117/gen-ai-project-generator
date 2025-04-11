# GPT-4o Project Generator

A powerful Python tool that leverages OpenAI's GPT-4o to automatically generate complete, production-ready fullstack project structures based on text descriptions. This tool acts as your AI development partner by creating organized directory structures and files with appropriate content to kickstart your development process.

## 🌟 Features

- **AI-Powered Project Creation**: Leverages OpenAI's GPT-4o model to design and create project structures
- **Multiple Project Types**: Supports various fullstack frameworks (MERN, MEAN, Django+React, Laravel+Vue, etc.)
- **Complete Project Structure**: Creates directories, files, configuration, and documentation
- **Production-Ready Templates**: Generates code templates following industry best practices
- **Safety-First Approach**: All operations are restricted to the current working directory
- **Secure by Design**: No sudo commands allowed for enhanced security
- **Detailed Summaries**: Provides comprehensive reports of what was created
- **Environment Variable Support**: Securely manages API keys via .env files
- **Interactive Terminal Interface**: Simple and user-friendly input process
- **Multiline Description Support**: Enter detailed project requirements with formatting

## 📋 Prerequisites

- Python 3.8 or higher
- OpenAI API key with access to GPT-4o
- Recommended: Virtual environment for isolation

## 🚀 Installation

1. Clone this repository:
```bash
git clone https://github.com/singhbipin2117/gen-ai-project-generator
cd gen-ai-project-generator
```

2. Create and activate a virtual environment (optional but recommended):
```bash
# For Linux/macOS
python -m venv venv
source venv/bin/activate

# For Windows
python -m venv venv
venv\Scripts\activate
```

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

4. Create a .env file in the project root:
```bash
echo "OPENAI_API_KEY=your-api-key-here" > .env
```

Replace `your-api-key-here` with your actual OpenAI API key.

## 📝 Usage

Simply run the generator and follow the interactive prompts:

```bash
python project_generator.py
```

You'll be prompted to provide:
1. The project type (e.g., "MERN Stack", "Django+React")
2. The project name
3. A detailed project description (supports multiple lines)

For the project description, type `END` on a new line when you've finished entering the description.

### Example Input Session

```
====================================================================================
GPT-4o PROJECT GENERATOR
====================================================================================
This tool will generate a complete project structure based on your specifications.
Please provide the following information:

Enter project type (e.g., MERN Stack, Django+React): MERN Stack
Enter project name: taskmanager

Enter project description (type 'END' on a new line when finished):
A task management application with user authentication, task creation, 
assignment, and tracking features. It should include:
- User registration and authentication
- Task creation with title, description, due date, priority, and assignee
- Dashboard with task statistics and visualizations
- RESTful API for all operations
- Responsive frontend design
END
```

## 🔧 Supported Project Types

The tool supports various project types out of the box:

- MERN Stack (MongoDB, Express, React, Node.js)
- MEAN Stack (MongoDB, Express, Angular, Node.js)
- Django+React
- Flask+Vue
- Laravel+React
- Next.js
- And many more!

## 📊 Project Summary

After generation, the tool provides a detailed summary including:

- Total files and directories created
- Generation time statistics
- Complete project structure
- Key features implemented
- A JSON summary file for future reference

## 🔒 Security Notes

- The generator only operates within the current working directory
- No sudo commands are allowed
- API keys are stored in environment variables or .env files
