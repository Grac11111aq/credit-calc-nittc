## Gemini CLI Agent Operational Guidelines

- **Long-running Commands**: For commands expected to run for more than 30 seconds (e.g., development servers, build processes), execute them in the background using `&`. Provide instructions for the user to retrieve logs at any time (e.g., by reading a log file or by providing a command to view the process output).
