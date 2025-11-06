# AI Crew for Game Building
## Introduction
This project demonstrates the use of the CrewAI framework to automate the creation of a game. CrewAI orchestrates autonomous AI agents, enabling them to collaborate and execute complex tasks efficiently.

By [@joaomdmoura](https://x.com/joaomdmoura)

- [CrewAI Framework](#crewai-framework)
- [Running the script](#running-the-script)
- [Details & Explanation](#details--explanation)
- [Contributing](#contributing)
- [Support and Contact](#support-and-contact)
- [License](#license)

## CrewAI Framework
CrewAI is designed to facilitate the collaboration of role-playing AI agents. In this example, The agents work together to build a Python-based game by simulating a collaborative software development process. Each agent has a distinct role, from writing the code to reviewing it for errors and ensuring it meets high-quality standards before final approval.


## Running the Script
It uses GEMINI (Free Version) by default so you should have access to that to run it. Sign up to [Google AI Studio](https://aistudio.google.com/) and create a FREE account along with a API key to use with this project. 


- **Configure Environment**: Copy `.env.example` and set up the environment variables for Gemini with [https://platform.openai.com/api-keys](https://aistudio.google.com/api-keys) . Import this env using `src .env.example`
- **Install Dependencies**: Run `poetry lock && poetry install` (uses crewAI==0.130.0).
- **Customize**: Modify `src/game_builder_crew/main.py` to add custom inputs for your agents and tasks.
- **Customize Further**: Check `src/game_builder_crew/config/agents.yaml` to update your agents and `src/game_builder_crew/config/tasks.yaml` to update your tasks.
- **Execute the Script**: Run `poetry run game_builder_crew` and input your project details.

## Details & Explanation
- **Running the Script**: Execute `poetry run game_builder_crew`. The script will leverage the CrewAI framework to generate a detailed job posting.
- **Key Components**:
  - `src/game_builder_crew/main.py`: Main script file.
  - `src/game_builder_crew/crew.py`: Main crew file where agents and tasks come together, and the main logic is executed.
  - `src/game_builder_crew/config/agents.yaml`: Configuration file for defining agents.
  - `src/game_builder_crew/config/tasks.yaml`: Configuration file for defining tasks.
  - `src/game_builder_crew/tools`: Contains tool classes used by the agents.


## License and Attribution

This project is licensed under the [MIT License](./LICENSE).

Portions of this codebase are derived from the
[CrewAI Examples Repository](https://github.com/agenticdevops/crewAI-examples),
which is licensed under the MIT License by the Agentic DevOps / CrewAI Team (c) 2024.

Modifications, integrations, and additional code contributions
are © 2025 The Linux Foundation.

