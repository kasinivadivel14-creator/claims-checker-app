# Club Expense Claim Checker

A beginner-friendly console Python project. It reads `claims.csv` and `budgets.csv`,
checks each claim, and creates four CSV reports in the `outputs` folder.

## Files
- `claims.csv`: example claims (20 rows)
- `budgets.csv`: category spending limits
- `main.py`: main application
- `system_prompt.txt`: LLM system prompt
- `payable.csv`: claims that passed all software checks
- `review.csv`: claims needing attention
- `results.csv`: all claims and statuses
- `summary.csv`: status counts and club/category budget totals

## Run in VS Code
1. Install Python 3 if it is not already installed.
2. Open this folder in VS Code.
3. Open Terminal > New Terminal.
4. Run `python -m pip install -r requirements.txt`.
5. Optional AI setup: copy `.env.example` to `.env`, then put your own API key after `OPENAI_API_KEY=`.
6. Keep `.env` private. It is excluded by `.gitignore`. Never upload it to GitHub.
7. Run `python main.py`.
8. Press Enter to use the default input names and output folder.

Without an API key, the program uses a basic fallback extractor. For the assessed
LLM requirement, configure a valid API key and test the LLM path.

## Important
This tool only classifies claims. It does not pay anyone. The faculty treasurer
must inspect the supporting document and sign every payment.

The assignment handout names `summary.txt`; this version uses `summary.csv`
because the project owner requested all four output reports in CSV format.
Ask faculty whether they accept this format change before final submission.
