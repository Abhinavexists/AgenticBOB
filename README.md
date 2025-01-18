# AgenticBOB 🤖

A powerful AI-powered content research and writing assistant built with CrewAI and Streamlit. AgenticBOB leverages multiple AI agents to conduct thorough research and generate high-quality content on any topic.

## Features

- Advanced web research capabilities using SerperDev API
- AI-powered content generation with multiple specialized agents
- Adjustable content parameters (temperature, style, format)
- Export content in multiple formats (Markdown, JSON)
- Source verification and fact-checking
- User-friendly Streamlit interface

## Quick Start

### Prerequisites

- Python 3.8+
- [Serper Dev API Key](https://serper.dev/)
- [OpenAI API Key](https://platform.openai.com/api-keys)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Abhinavexists/AgenticBOB.git
cd AgenticBOB
```

2. Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the project root and add your API keys:
```env
OPENAI_API_KEY=your_openai_api_key
SERPER_API_KEY=your_serper_api_key
```

### Running the Application

1. Start the Streamlit app:
```bash
streamlit run app.py
```

2. Open your browser and navigate to `http://localhost:8501`

## Usage

1. Enter your desired content topic in the sidebar
2. Adjust the temperature slider to control creativity level
3. Click "Generate Content" to start the process
4. Wait for the AI to generate your article
5. Download the result as a markdown file

## How It Works

AgenticBOB uses two specialized AI agents:

### Senior Research Analyst
- Conducts comprehensive web research
- Evaluates source credibility
- Fact-checks information
- Creates structured research briefs

### Content Writer
- Transforms research into engaging content
- Maintains factual accuracy
- Creates well-structured articles
- Includes proper citations

## Project Structure

```
AgenticBOB/
├── .env                # Environment variables
├── app.py              # Streamlit web application
├── main.py             # Core logic and agent definitions
├── requirements.txt    # Project dependencies
└── README.md           # Project documentation
```

## Configuration

You can modify the following parameters:

- `temperature`: Controls creativity level (0.0 - 1.0)
- `n_results`: Number of search results to process (default: 10)
- `timeout`: Maximum processing time (default: 120s)
- `max_tokens`: Maximum output length (default: 4000)

## 🛠️ Advanced Usage

### Running from Command Line
You can also run the content generation directly from the command line:

```bash
python main.py "Your topic here"
```

### Customizing Agents
Modify `main.py` to adjust agent parameters:
- Change agent goals and backstories
- Add new tools and capabilities
- Modify output formats and requirements

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the GNU License - see the [LICENSE](LICENSE) file for details.