GPT-4o Project Generator
A powerful Python tool that leverages OpenAI's GPT-4o to automatically generate complete, production-ready fullstack project structures based on text descriptions. This tool acts as your AI development partner by creating organized directory structures and files with appropriate content to kickstart your development process.

🌟 Features

AI-Powered Project Creation: Leverages OpenAI's GPT-4o model to design and create project structures
Multiple Project Types: Supports various fullstack frameworks (MERN, MEAN, Django+React, Laravel+Vue, etc.)
Complete Project Structure: Creates directories, files, configuration, and documentation
Production-Ready Templates: Generates code templates following industry best practices
Safety-First Approach: All operations are restricted to the current working directory
Secure by Design: No sudo commands allowed for enhanced security
Detailed Summaries: Provides comprehensive reports of what was created
Environment Variable Support: Securely manages API keys via .env files

📋 Prerequisites

Python 3.8 or higher
OpenAI API key with access to GPT-4o
Recommended: Virtual environment for isolation

🚀 Installation

Clone this repository:

bashgit clone https://github.com/yourusername/gpt4o-project-generator.git
cd gpt4o-project-generator

Create and activate a virtual environment (optional but recommended):

bash# For Linux/macOS
python -m venv venv
source venv/bin/activate

# For Windows
python -m venv venv
venv\Scripts\activate

Install required dependencies:

bashpip install -r requirements.txt

Create a .env file in the project root:

bashecho "OPENAI_API_KEY=your-api-key-here" > .env

Replace your-api-key-here with your actual OpenAI API key.

📝 Usage
Basic Usage
Run the generator with default settings:
bashpython project_generator.py
This will create a MERN stack project named "taskmanager" in your current directory.
Customizing Project Generation
To create a custom project, modify the main() function in project_generator.py:
python# Define project details
project_type = "Django+React"  # Change to your desired framework
project_name = "my_awesome_project"  # Change to your desired project name
project_description = """
A blog platform with user authentication, post creation, comments,
and rich text editing. It should include:
- User registration and authentication with social logins
- Post creation with categories and tags
- Comments with threading and moderation
- Admin dashboard for content management
- Responsive design for mobile and desktop
- Deployment configuration for AWS
"""  # Provide a detailed description

# Generate the project
result = generator.generate_project(project_type, project_name, project_description)
