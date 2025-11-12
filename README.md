# sm-semantic-kernel-examples

A collection of examples demonstrating the capabilities of Microsoft Semantic Kernel with local AI models via LM Studio. This project showcases various AI-driven tasks such as chat completion, text summarization, and data analysis using a console application built with .NET 8.0.

## Prerequisites

- [.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0) or later
- [LM Studio](https://lmstudio.ai/) installed and running locally
- A compatible model downloaded in LM Studio (e.g., deepseek/deepseek-r1-0528-qwen3-8b)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/sm-semantic-kernel-examples.git
   cd sm-semantic-kernel-examples
   ```

2. Restore NuGet packages:
   ```bash
   dotnet restore
   ```

## Setup

1. **Install and Start LM Studio:**
   - Download and install LM Studio from [lmstudio.ai](https://lmstudio.ai/)
   - Launch LM Studio and download the required model (deepseek/deepseek-r1-0528-qwen3-8b)
   - Start the local server in LM Studio (typically runs on http://localhost:1234)

2. **Verify Model Configuration:**
   - Ensure the model is loaded and the server is running on the expected endpoint
   - The application is configured to connect to `http://localhost:1234/v1`

## Usage

Run the console application to execute all examples:

```bash
dotnet run --project ConsoleApp1
```

The application will run four examples sequentially, demonstrating different AI capabilities.

## Examples

### Example 1: Rhyming Day Check
Demonstrates chat completion with a system prompt that enforces rhyming responses. The AI is instructed to always answer in rhymes and is given context that today is Thursday.

### Example 2: Text Summarization
Shows how to use Semantic Kernel for summarizing text. It takes a description of Semantic Kernel and generates a concise summary using the local AI model.

### Example 3: Number Analysis
Analyzes a list of numbers to find patterns, calculate averages, and describe trends. Demonstrates data analysis capabilities of the AI model.

### Example 4: Number Analysis & Prediction
Extends the number analysis by predicting the next number in a sequence. Shows advanced pattern recognition and predictive capabilities.

## Dependencies

- Microsoft.SemanticKernel v1.67.1

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
