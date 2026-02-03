⚙️ Execution Process with Ollama /


**What is Ollama** /
-Ollama is a lightweight framework for running large language models (LLMs) locally. It manages models, authentication, and background processes through a daemon.

**What is Daemon?** /
-The daemon is a computer program that runs in background, without a user interface or command line interface.
-In simple, it is the server that does the work.
- On Windows, Ollama runs automatically in the background when you use commands like ollama run.
- You interact with Ollama entirely through the command line interface (CLI).

**Starting Ollama** /
- Normally, the daemon starts automatically when you run any Ollama command.
- To start manually:
    -> ollama serve
(If you see a port binding error, it means the daemon is already running.)

**Common Commands and Usage**
serve - Start ollama /
create - Create a model /
show - show information for a model /
run - run a model /
stop - stop running a model /
pull - pull a model from a registry /
push - push a model from a registry /
signin - signin to ollama.com /
signout - signout from ollama.com /
list - list models /
ps - list running models /
rm - remove a model which is installed /
launch - launch an integration with ollama /
help - help about any command /

**Example Workflow**
# 1. Pull a model
ollama pull llama2

# 2. Run interactively
ollama run llama2

# 3. Exit session
/bye   # or Ctrl+C

# 4. Check running processes
ollama ps

# 5. Stop model if still active
ollama stop llama2

# 6. List installed models
ollama list



**Learnings & Takeaways**
- Using Hugging Face models in Python
- Generating & managing access tokens securely
- Integrating Hugging Face with local environments
- Connecting Google Colab with VS Code for flexible workflows
- Launching Gradio apps directly from notebooks
- Running and managing Ollama models locally with CLI commands

**Future Improvements**
- Add support for multiple Hugging Face models (text, vision, audio)
- Dockerize the application for easier deployment
- Extend authentication setup for production environments
- Enhance UI with custom Gradio components
- Explore advanced Ollama workflows with custom models