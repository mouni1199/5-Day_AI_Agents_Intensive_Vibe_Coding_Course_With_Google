# Antigravity
**Google Antigravity is a comprehensive, agent-first development ecosystem designed to build, orchestrate, and deploy autonomous AI agents.**

## Antigravity ecosystem :
**1.Antigravity 2.0:**
* Standalone application runs on windows,linux,macOS 
* command center to manage multiple agents in parallel
* runs scheduled tasks
* functions independently without IDE

**2.Antigravity IDE:**
* original fully-featured agentic IDE
* Equipped with built-in agent management, artifact handling 
* advanced code-context understanding.

**3.Antigravity CLI:**
* Terminal based interface 
* Use the terminal to interact with your agents

**4.Antigravity SDK:**
* Build and integrate Antigravity programmatically.
* Connect Antigravity to your systems.
* Integrate Antigravity via developer tools.
* Programmatically implement Antigravity into workflows.

## Antigravity_Projects
**Antigravity uses a project-centric approach to ensure the agents have access to the right files, tools, permissions and more**
* A project is a combination of folders defining the environment and the scope of your agent.
* it can work with one or multiple folders, providing your agents with all of the context required for your codebase.
* All projects have their own isolated agent settings, allowing you to customize different projects' security settings independently.

### Project settings 
* **Security preset :** 
    *   Controls terminal auto execution and file access policy
    *   All the terminal commands and file accesses require manual review before any action performed by agent.
* **Agent Behaviour :**
    *   Implementation plan would be executed with or without user review.
* **Local Permissions :**
    *   Files, URL's access allowed for agent or not.
* MCP tools can be configured per project(as needed) instead of using all the servers that are globally configured.

## Slash Commands
* Text based short-cuts that triggers specific actions,workflows or tools within an application.
    - Ex :- /browser - it is an explicit command to launch browser. Triggers sub-agent which needs google chrome and permission for debugging.
            /schedule - used for repetative tasks at particular intervals (execute task on 9:00 AM on Monday, Wednesday) 

## Scheduling commands
* Schedule option in the main interface to automate recurring tasks or set one-time reminders in your specific projects.
    *   Used through GUI(Schedule task) or /schedule command 
    *   Can set cron-style instructions(hourly,daily,weekly,or custom times) to orchestrate multi-agent workflows 

## **MCP:**
***The Model Context Protocol (MCP) is an open-source standard that connects AI applications seamlessly to external data sources, tools, and workflows.***
* **Core Architecture :**
    MCP eliminates the need for messy API integrations by using a standardized Client-Server architecture over JSON-RPC 2.0:
    *   **MCP Host**: The application running the AI, such as a desktop chat app (e.g., Claude Desktop) or a coding editor
    *   **MCP Client**: A helper module within the Host that manages security, negotiates capabilities, and translates the AI's requests into protocol messages.
    *   **MCP Server**: : A lightweight, standalone program that bridges the client to a specific data source or service, such as GitHub, Slack, or a local database.



