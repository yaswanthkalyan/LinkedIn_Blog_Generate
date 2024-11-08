
# LinkedIn Post Generator

This project is a LinkedIn Post Generator built using Python, Streamlit, and a language model (`llm_helper`). It allows users to create customized LinkedIn posts based on selected parameters like topic, length, and language. This app is designed to generate engaging and topic-focused LinkedIn posts quickly and efficiently.

## Features

- **Dynamic Post Generation**: Create LinkedIn posts on various topics with selected lengths and languages.
- **Few-shot Learning**: Incorporates examples to guide the language model in generating posts with a relevant style and tone.
- **User-friendly Interface**: Interactive dropdowns for selecting topic, length, and language.
- **Multi-language Support**: Choose between English and Hinglish for post generation.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yaswanthkalyan/LinkedIn_Blog_Generator.git
   cd linkedin-post-generator
   ```

2. **Install Dependencies**:
   Make sure you have Python 3.8 or above installed. Install required packages using:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   Start the Streamlit app using:
   ```bash
   streamlit run app.py
   ```

## Usage

1. **Select Topic**: Choose a topic (tag) for the LinkedIn post from the dropdown.
2. **Select Length**: Define the length of the post (`Short`, `Medium`, or `Long`).
3. **Select Language**: Choose between `English` and `Hinglish`.
4. **Generate Post**: Click the "Generate" button to create a customized LinkedIn post, which will appear below the options.

## Code Overview

### Key Files

- **`app.py`**: Main Streamlit application file that manages the UI and integrates functions.
- **`llm_helper.py`**: Manages the language model (LLM) integration.
- **`few_shots.py`**: Provides examples (few-shot examples) to guide the language model in generating consistent and high-quality content.
- **`post_generator.py`**: Contains core functions for generating and structuring LinkedIn post prompts.

### Key Functions

- **`generate_post(length, language, tag)`**: Generates a LinkedIn post based on the user's selections.
- **`get_prompt(length, language, tag)`**: Constructs a prompt for the language model using selected options and few-shot examples.
- **`get_length_str(length)`**: Converts the length option into a specific range of lines (1-5, 6-10, or 11-15).

## Future Improvements

- **Caching**: Cache dropdown options and previous responses to improve performance.
- **Error Handling**: Add error handling for better user feedback if post generation fails.
- **Customizable Examples**: Allow users to customize the number of examples used in few-shot prompts.
- **Enhanced Customization**: Add options for tone (formal/informal) and post structure (bullet points, numbered lists).

## Contributing

If you'd like to contribute, please fork the repository and make a pull request. For major changes, open an issue to discuss your ideas.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.



Enjoy generating LinkedIn posts and engage your audience with ease!
