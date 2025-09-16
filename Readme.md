AI agents Demo
--------------

- [About](#about)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Launch examples](#launch-examples)
  - [Check correct configuration](#check-correct-configuration)
  - [Run agents demos](#run-agents-demos)



# About

Is it difficult to work with agents? Do I need a lot of experience? Well, as always happens with complex questions, the most reasonable answer is: it depends. A full enterprise-grade project with multiple services and data integrations is difficult, but a small proof of concept to learn the technology and the tools it is not. This is what we are going to learn today. We will use **Crew.AI**, **Perplexity** and **Nano banana** to create autonomous agents that enrich our articles with stunning visualizations.


# Requirements

We are going to work with AI agents, for this **you need access to an LLM**. Here we have selected Perplexity's hosted models, but you can use any other provider such as Groq, AWS Bedrock or even hosting it in local. The examples and guides here will show you how to use the Perplexity option. Thus you need a **internet connection** and a **Perplexity account with tokens or credits** available.

Tip: these days there are some promos to get a free trial for Perplexity Pro and that tier includes free monthly credits. Use Google ;-)

A **Python** environment is required as well. We will use Anaconda to work with virtual environments, but feel free to choose any option desired.

# Installation

You can create the environment and install the dependencies like this:

```bash
conda create -n "agent_demo" python=3.12
conda activate "agent_demo"
pip install -r requirements.txt
```

# Configuration

1. Rename the file `.env.template` to just `.env`
2. Insert your API key in the new `.env` file.

Simple and easy.

# Launch examples

## Check correct configuration

To make sure the experience is as smoother as it should be, there are a couple of notebooks to check that all configurations are correct. When you achieve this milestone you can go directly to the agent's stuff and start with the fun without any typical error or random explosions.

In this path: `notebooks/configuration_tests/` you will find:

1. `test_perplexity.ipynb`: here you will test that you can use Perplexity's LLM. That you have tokens, that you have correctly configured an API key, etc.
2. `test_crewai.ipynb`: once Perplexity configuration is ready you can check its integration with Crew.AI.

If you could run successfully both notebooks it means you are ready for the best part: agents!!

## Run agents demos

Do you know that you can unlock the power of autonomous agents... from a simple jupyter notebook in your laptop? Let's get our hands dirty.

In `notebooks/agents` you will find:

1. `illustrator_agent.ipynb` which contains a full example of how to use an autonomous agent to illustrate an article.
2. `illustrator_multi_agent.ipynb` which contains the skeleton of a semi-functional example of how to create a crew of multiple agents to collaborate illustrating an article




