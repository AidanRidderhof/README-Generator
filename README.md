# README-Generator 📝

[![Python](https://img.shields.io/badge/python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

---

## Table of Contents
- [About](#about)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## About

**README-Generator** is a Python-based tool that leverages GitHub and OpenAI APIs to automatically generate professional README files for GitHub repositories. By analyzing your repository’s file structure and content, it creates meaningful documentation, saving you time and improving project visibility.

Built with an interactive Gradio interface, it’s easy to use and integrates environment variables for secure API key management.

---

## Features ✨

- 🔗 **GitHub Repository Parsing**  
  Extracts owner and repository name from any valid GitHub URL.

- 🌲 **Repository Tree Retrieval**  
  Fetches the complete file structure from the default branch recursively using GitHub API.

- 📄 **Important File Filtering**  
  Focuses on key source code files with extensions like `.py`, `.js`, `.ts`, `.go`, `.java`, `.cpp`, and more.

- 🤖 **OpenAI Integration**  
  Uses OpenAI’s API to generate meaningful README content based on repository files.

- 🎨 **Interactive UI with Gradio**  
  Provides an easy-to-use web interface for inputting repository URLs and viewing generated README outputs.

- 🔐 **Secure API Key Management**  
  Loads GitHub and OpenAI API keys from environment variables using `dotenv`.

---

## Installation 🚀

1. **Clone the repository**

   ```bash
   git clone https://github.com/AidanRidderhof/README-Generator.git
   cd README-Generator
   ```

2. **Create and activate a virtual environment (optional but recommended)**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**

   Create a `.env` file in the root directory and add your API keys:

   ```env
   GITHUB_TOKEN=your_github_token_here
   OPENAI_API_KEY=your_openai_api_key_here
   ```

---

## Usage 💡

Run the Jupyter notebook `readMe-Generator.ipynb` to launch the Gradio interface:

```bash
jupyter notebook readMe-Generator.ipynb
```

Or, if you prefer, you can extract and adapt the code to run as a standalone Python script.

### How to generate a README:

1. Enter the full GitHub repository URL (e.g., `https://github.com/owner/repo`) into the input field.
2. Submit and wait for the tool to analyze the repository.
3. View and copy the generated README content.

---

## Contributing 🤝

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/README-Generator/issues).

To contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request

Please make sure to update tests as appropriate.

---

## License 📄

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---
*Made with ❤️ using Python, GitHub API, and OpenAI*
