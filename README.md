# DebageGPT - Autonomous AI Debate Opponent

## Introduction

This project presents an autonomous AI agent designed to engage in debates by leveraging the power of Large Language Models (LLMs) and speech recognition/synthesis technologies. The agent is capable of understanding and responding to debates in a structured manner, providing support in various stages of a debate, from introduction to conclusion. It is an innovative tool that can significantly enhance the quality of debates by offering strategic arguments, counterarguments, and rebuttals, all generated by an AI with a focus on logical consistency and persuasive power.

## Use Case

The primary use case for this project is to serve as a debating opponent for individuals or teams participating in debates, particularly in educational or public speaking contexts. It can be particularly useful in scenarios where participants are looking to strengthen their arguments through logical reasoning and evidence-based counterarguments. By leveraging AI, this tool ensures that debaters can train themselves to present their arguments more effectively, by providing them with well-structured responses that are both logically sound and persuasive.

## Features

- **Speech Recognition**: Utilizes the `speech_recognition` library to convert spoken language into text, enabling real-time interaction in debates.
- **Text-to-Speech**: Employs `pyttsx3` for converting text responses into spoken words, facilitating auditory engagement in the debate.
- **Debate Structure**: Follows a predefined structure for debates, including introduction, presentation of arguments, counter-arguments, rebuttals, summarization, and conclusion.
- **AI-Generated Responses**: Leverages the power of LLMs to generate responses that are contextually relevant, logically sound, and persuasive.
- **Stage Detection**: Capable of determining the current stage of a debate and suggesting appropriate responses or actions.

## Getting Started

To get started with this project, you will need to:

1. Install the required libraries (`speech_recognition`, `pyttsx3`, `whisper`, `requests`, and `json`).
2. Obtain an API key for the Perplexity AI service to access the LLM.
4. Set up the environment variables for the Perplexity API key.
5. Determine debate_topic and debater_viewpoint.
7. Run the `debategpt.py` and debate against LLM, use with_sound=True to debate with actual speech (using Whisper and Pyttsx3) and with_sound=False to debate in CLI format.

## Example Usage

```python
debate_topic: str = "Should the government provide a guaranteed basic income for all citizens."
debater_viewpoint: str = "A guaranteed basic income is bad, because it makes people dependent on government, reduces incentives for work and entrepreneurship, gives too much power to the government."

debate(debate_topic, debater_viewpoint, with_sound=True)
```

## Contributing

Contributions to enhance the functionality, improve the debate structure, or integrate additional AI models are welcome. Please follow the standard GitHub workflow: fork, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgements

This project is inspired by the advancements in AI and natural language processing, particularly the capabilities of Large Language Models. We appreciate the contributions of the AI research community and the open-source community for making such technologies accessible.
