# 🚀 Roadmap Generator

A powerful CLI tool that helps developers and project managers create comprehensive project roadmaps using Claude AI, with support for custom prompts and multiple output formats.

## ✨ Features

- 🤖 **AI-Powered Generation** - Create detailed roadmaps using Claude 3 Sonnet
- 📝 **Custom Prompts** - Use specialized prompts for different project types
- 📊 **Structured Output** - Get well-organized, hierarchical project plans
- 🎯 **Project Phases** - Automatically break down projects into logical phases
- 💾 **Multiple Formats** - Export roadmaps in markdown format
- 🔄 **Interactive Mode** - Refine roadmaps through conversation with AI
- 🎬 **Customizable Animations** - Choose from different loading animations

## 📋 Requirements

- Python 3.10+
- Anthropic API key

## 🔧 Installation

### Option 1: Install from Source

```bash
# Clone the repository
git clone https://github.com/pkells12/roadmap-generator.git
cd roadmap-generator

# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## ⚙️ Configuration

1. Copy the example environment file:
   ```bash
   cp env.example .env
   ```

2. Edit the `.env` file and add your Anthropic API key:
   ```
   ANTHROPIC_API_KEY=your_api_key_here
   ```

   You can get an API key by signing up at [Anthropic](https://www.anthropic.com/).

## 🚀 Usage

The Roadmap Generator provides two main commands:

### Generate a Roadmap and Display It

```bash
python main.py generate "Your app idea description"
```

This command generates a roadmap based on your app idea and displays it in the terminal.

### Generate a Roadmap and Save It to a File

```bash
python main.py save "Your app idea description" --output-file project_roadmap.md
```

This command generates a roadmap and saves it to the `roadmaps` directory with the specified filename.

### Command Options

Both commands support the following options:

- `--animation`: Choose the loading animation type (spinner, dots, bar, typing)
  ```bash
  python main.py generate "Your app idea description" --animation typing
  ```

### Examples

#### Generate a Simple Web App Roadmap

```bash
python main.py generate "A to-do list web app with user authentication, task categories, and reminders"
```

#### Generate a Mobile App Roadmap and Save It

```bash
python main.py save "A fitness tracking mobile app that records workouts, tracks progress, and provides workout recommendations" --output-file fitness_app_roadmap.md
```

#### Generate a Roadmap with a Custom Animation

```bash
python main.py generate "An e-commerce platform for selling handmade crafts" --animation bar
```

## 📁 Output

Generated roadmaps are saved to the `roadmaps` directory by default. You can specify a custom filename with the `--output-file` parameter.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

MIT 