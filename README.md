# Patient Simulation Prototype

## Overview

This project is an early-stage **AI-powered patient simulation prototype** created to explore how conversational AI and immersive technology could support nursing education.

The project includes two main prototype directions:

* A **chat-based patient simulation**, where a learner can interact with an AI-powered virtual patient through conversation.
* An early **Unity/Oculus prototype**, where a virtual patient image was displayed in a VR environment to explore how patient scenarios could eventually be presented immersively.

The goal of the project was to experiment with different ways nursing students could interact with simulated patients in a safe learning environment.

## Chat-Based Prototype

The chat-based prototype allows users to communicate with a simulated patient using natural language.

The system is designed so that a learner can:

* Ask the virtual patient questions
* Gather information about the patient's condition
* Practice conversational assessment
* Work through a simulated clinical interaction

The prototype uses a configurable large language model through the settings provided in the configuration file.

## Text-to-Speech

The project also includes support for text-to-speech using **XTTS v2**.

Example configuration:

```yaml
tts:
  use_gpu: false
  model_name: 'tts_models/multilingual/multi-dataset/xtts_v2'
  speaker: 'Rosemary Okafor'
  language: 'en'
```

The configuration also supports optional streaming and voice-cloning settings.

## LLM Configuration

LLM settings are stored in the configuration file using placeholders:

```yaml
llm:
  model: "YOUR_MODEL"
  api: "YOUR_API"
  api_key: "YOUR_KEY"
  system_message: "You are a helpful assistant."
  temperature: 0.7
  top_p: 0.9
```

Replace these values locally with the model and API service you are using.

**Do not commit real API keys or private service credentials to the repository.**

## Unity / VR Exploration

A separate Unity-based prototype was created to explore the immersive side of the project.

During this stage, a virtual patient visual was successfully displayed through an **Oculus headset**. This served as an initial proof of concept for how a patient simulation could eventually be experienced in a VR environment.

The VR portion should be considered an exploratory prototype rather than a complete interactive nursing simulation.

## Technologies Explored

* Python
* Large Language Models
* Conversational AI
* XTTS v2
* Text-to-Speech
* Unity
* Oculus / Virtual Reality
* AI-assisted healthcare education

## Project Context

This project was developed during **Spring 2026 at UNC Charlotte** as part of an exploration of AI-supported nursing simulation.

The experience focused on rapid prototyping and investigating how conversational AI and immersive environments could potentially be used to support healthcare education.

## Disclaimer

This project is an **educational and research prototype**.

It is not intended for clinical use, medical diagnosis, treatment recommendations, or real-world patient care.
