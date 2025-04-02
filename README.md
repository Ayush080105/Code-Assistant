# AI Code Assistant

This is a simple AI-powered code assistant using Code Llama. It takes user input as a coding problem and generates responses using a locally hosted Code Llama model via API calls.

## Features
- Accepts coding-related queries from users.
- Generates responses based on the provided prompt.
- Maintains conversation history for better context.
- Uses Gradio for an interactive user interface.

## Requirements
- Python 3.8+
- Required Python libraries:
  - `requests`
  - `json`
  - `gradio`

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/ai-code-assistant.git
   cd ai-code-assistant
   ```

2. Install dependencies:
   ```sh
   pip install requests gradio
   ```

3. Ensure Code Llama is running locally on port 11434.

## Usage

1. Run the AI Code Assistant:
   ```sh
   python app.py
   ```

2. Open the Gradio interface in your browser and enter your coding problem.

## Code Explanation

### `generate_response(prompt)`
- Maintains a history of prompts to provide context.
- Sends a request to the locally running Code Llama API (`http://localhost:11434/api/generate`).
- Processes the JSON response and returns the generated code.

### Gradio Interface
- Uses `gr.Interface` to create an interactive UI.
- Accepts user input via a text box.
- Displays the generated response as output.

## Contribution
Feel free to contribute by submitting issues or pull requests. If you encounter any problems, let us know!

## License
This project is licensed under the MIT License.

