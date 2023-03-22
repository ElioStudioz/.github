## Hi there 👋

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
.DEFAULT_GOAL := help

.PHONY: help

help: ## Display this help message

	@awk 'BEGIN {FS = ":.*##"; printf "\nUsage:\n  make \033[36m<target>\033[0m\n\nTargets:\n"} /^[a-zA-Z_-]+:.*?##/ { printf "  \033[36m%-30s\033[0m %s\n", $$1, $$2 }' $(MAKEFILE_LIST)

readme: ## Generate unique README.md content

	@echo "# ElioStudioz\n\nWelcome to ElioStudioz, a community-driven organization that focuses on creating Discord bots using different programming languages and libraries. Our aim is to provide high-quality bot projects that can be used as a starting point for your own projects or as a source of inspiration for new ideas.\n\n## Our Projects\n\nHere are some of the projects we have worked on:\n\n- Project 1: Description of the project and its features\n- Project 2: Description of the project and its features\n- Project 3: Description of the project and its features\n\n## How to Contribute\n\nWe welcome contributions from everyone, regardless of their skill level or experience. Here are some ways you can contribute:\n\n- Report bugs or issues you encounter\n- Suggest new features or improvements\n- Submit pull requests to fix bugs or add new features\n- Help with documentation and tutorials\n\nIf you are interested in contributing, please read our [Contribution Guidelines](CONTRIBUTING.md) and join our [Discord server](https://discord.gg/elio) to get in touch with our team.\n\nThank you for visiting ElioStudioz, and we hope you find our projects useful!"
