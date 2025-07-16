# UPSC-Essay-workflow

# UPSC Essay Evaluation Workflow

This project implements an automated essay evaluation system specifically designed for UPSC (Union Public Service Commission) exam preparation. It uses LangGraph and Google's Gemini AI model to provide comprehensive feedback on essays.

## Features

- **Multi-dimensional Evaluation**: Assesses essays based on:
  - Language Quality
  - Depth of Analysis
  - Clarity of Thought
  - Overall Feedback
- **Structured Output**: Returns detailed feedback with numerical scores (0-10) for each category
- **Workflow Management**: Uses LangGraph to manage the evaluation workflow
- **AI-Powered**: Leverages Google's Gemini 1.5 Pro model for nuanced essay assessment

## Prerequisites

- Python 3.8+
- Google Gemini API key (set as environment variable `GEMINI_API_KEY`)
- Required Python packages (see `requirements.txt`)

## Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your Google Gemini API key as an environment variable:
   ```bash
   export GEMINI_API_KEY='your-api-key-here'
   ```

## Usage

1. Open the Jupyter notebook `5_UPSC_essay_workflow.ipynb`
2. Run the notebook cells to initialize the evaluation workflow
3. Input your essay text in the designated cell
4. Execute the workflow to get detailed feedback and scores

## Evaluation Criteria

1. **Language Quality**: Grammar, vocabulary, and writing style
2. **Depth of Analysis**: Insightfulness and thoroughness of arguments
3. **Clarity of Thought**: Logical flow and coherence of ideas
4. **Overall Feedback**: Comprehensive assessment and suggestions

## Example Output

The system provides structured feedback in the following format:

```json
{
  "language_feedback": "Detailed feedback on language aspects...",
  "analysis_feedback": "Feedback on depth of analysis...",
  "clarity_feedback": "Assessment of thought clarity...",
  "overall_feedback": "Comprehensive evaluation summary...",
  "individual_scores": [8, 7, 9],
  "avg_score": 8.0
}
```

## Customization

You can modify the evaluation criteria and weights by adjusting the `EvaluationSchema` class in the notebook.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Google Gemini for the AI language model
- LangGraph for workflow management
- UPSC for the evaluation framework
