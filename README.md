# Obsidian LLM Summary Plugin

Obsidian LLM Summary Plugin is a simple community plugin that allows you to generate short summaries of selected text inside your notes using a hosted Large Language Model (LLM).

This plugin is an early version and focuses on providing a minimal summarization workflow directly inside Obsidian.

---

## Features

- Summarize any selected text in your notes
- Uses the Hugging Face Inference API
- Powered by the `Falconsai/text_summarization` model
- Lightweight and easy to configure

---

## How It Works

When you select text and trigger the summarizer command, the plugin sends the selected text to Hugging Face’s hosted API endpoint, which generates a summary using the Falconsai model.

This means summarization is performed externally (not locally on your device).

---

## Installation

### Manual Installation

1. Download or clone this repository
2. Copy the plugin folder into:

   `<YOUR VAULT>/.obsidian/plugins/llm-summary`

3. Restart Obsidian
4. Enable the plugin from:

   **Settings → Community Plugins → Installed Plugins**

---

## Setup

To use the plugin, you must provide your own Hugging Face API token.

### Steps:

1. Go to Hugging Face token settings:

   https://huggingface.co/settings/tokens

2. Generate a new access token

3. Open Obsidian settings:

   **Settings → LLM Summary Plugin**

4. Paste your token into the plugin settings

5. Press validate to validate the token.
---

## Usage

1. Select any text inside a note
2. Right-click the selection
3. Choose:

   **Falcon Summarizer**

4. The plugin will display a generated summary inside a modal window

---

## Model & API Attribution

This plugin uses the Hugging Face Inference API to generate summaries via the following model:

- **Model:** [`Falconsai/text_summarization`](https://huggingface.co/Falconsai/text_summarization)

This project is not affiliated with or endorsed by Hugging Face or Falconsai.

---

## Privacy Notice

Selected text is sent to Hugging Face’s hosted servers for processing.

Please avoid submitting sensitive, private, or confidential information.

Users are responsible for managing their own Hugging Face API token.

---

## Roadmap

Planned improvements include:

- Support for multiple summarization models
- Custom summary length controls
- Better UI integration

---

## License

This plugin is released under the MIT License.

---

## Author

Created as a first community plugin project for Obsidian.

Contributions, feedback, and suggestions are welcome.
