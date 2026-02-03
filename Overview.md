**Execution Process with Ollama** 


**What is Ollama**


-Ollama is a lightweight framework for running large language models (LLMs) locally. It manages models, authentication, and background processes through a daemon.

**What is Daemon?**


-The daemon is a computer program that runs in background, without a user interface or command line interface.
-In simple, it is the server that does the work.
- On Windows, Ollama runs automatically in the background when you use commands like ollama run.
- You interact with Ollama entirely through the command line interface (CLI).

**Starting Ollama**


- Normally, the daemon starts automatically when you run any Ollama command.
- To start manually:
    -> ollama serve
(If you see a port binding error, it means the daemon is already running.)

**Common Commands and Usage**


**serve** - Start ollama


**create** - Create a model


**show** - show information for a model


**run** - run a model 


**stop** - stop running a model 


**pull** - pull a model from a registry 


**push** - push a model from a registry 


**signin** - signin to ollama.com


**signout** - signout from ollama.com 


**list** - list models 


**ps** - list running models 


**rm** - remove a model which is installed 


**launch** - launch an integration with ollama 


**help** - help about any command 



**Example Workflow**


**1. Pull a model**
ollama pull llama2

**# 2. Run interactively**
ollama run llama2

**# 3. Exit session**
/bye   # or Ctrl+C

**# 4. Check running processes**
ollama ps

**# 5. Stop model if still active**
ollama stop llama2

**# 6. List installed models**
ollama list



**Learnings & Takeaways**

**Client-Server Architecture:** Understanding how the Daemon acts as a background server while the CLI functions as the client—a crucial concept for debugging local AI.


**Resource Management:** Learning how to manage RAM and GPU usage when swapping between different model sizes (e.g., 7B vs. 13B parameters).


**Process Control:** Mastering CLI commands like ps, kill, and serve to manually control model instances and resolve port binding errors.

