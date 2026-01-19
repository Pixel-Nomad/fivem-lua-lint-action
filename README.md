# 🧠 FiveM Luacheck Action
This project provides a GitHub Action for running luacheck on a project with FiveM natives. It allows developers to easily integrate luacheck into their GitHub Actions workflow, ensuring that their Lua code is checked for errors and follows best practices. The action is highly customizable, supporting features like capturing output, failing on warnings, and using extra libraries.

## 🚀 Features
- **Customizable**: The action allows developers to customize the luacheck execution by providing input parameters such as arguments, paths, and configuration files.
- **Integration with FiveM API**: The action fetches data from the FiveM API to generate a configuration file for luacheck, ensuring that the check is tailored to FiveM natives.
- **Support for extra libraries**: Developers can specify extra libraries to be used during the luacheck execution, making it easy to include custom or third-party libraries in the check.
- **Capturing output and failing on warnings**: The action supports capturing the output of the luacheck execution and failing the workflow if warnings are encountered, ensuring that developers are notified of potential issues.

## 🛠️ Tech Stack
- **GitHub Actions**: The action is built on top of GitHub Actions, providing a seamless integration with GitHub workflows.
- **Docker**: The action uses a Docker image to run the luacheck execution, ensuring a consistent and isolated environment.
- **TypeScript**: The project uses TypeScript for development, providing a robust and maintainable codebase.
- **Node.js**: The project uses Node.js as the runtime environment, providing a flexible and scalable platform.
- **Luacheck**: The action uses luacheck as the linter, providing a comprehensive check for Lua code.
- **FiveM API**: The action integrates with the FiveM API to fetch data and generate a configuration file for luacheck.

## 📦 Installation
To use this action in your GitHub Actions workflow, you'll need to:
1. **Create a new workflow file**: Create a new file in your repository's `.github/workflows` directory, e.g., `.github/workflows/luacheck.yml`.
2. **Add the action**: Add the following code to your workflow file:
```yml
name: Luacheck
on: [push, pull_request]
jobs:
  luacheck:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v2
      - name: Run luacheck
        uses: ./action.yml
```
3. **Configure the action**: Configure the action by providing input parameters such as arguments, paths, and configuration files.

## 💻 Usage
To use the action, simply trigger the workflow by pushing code changes to your repository or creating a pull request. The action will run automatically, checking your Lua code for errors and warnings.

## 📂 Project Structure
```markdown
.
├── action.yml
├── generate-rc.ts
├── Dockerfile
├── package.json
├── tsconfig.json
└── ...
```

## 📸 Screenshots


## 🤝 Contributing
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and submit a pull request with your changes.

## 📝 License
This project is licensed under the MIT License.

## 📬 Contact
For questions or issues, please contact us at [support@example.com](mailto:support@example.com).

## 💖 Thanks Message
Thanks for using our FiveM Luacheck Action! This is written by [readme.ai](https://readme-generator-phi.vercel.app/)
