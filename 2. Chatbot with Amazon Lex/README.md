# AWS Chatbot with Amazon Lex, Lambda, and CloudFormation

This project builds a BankingBot that helps users check their account balances and transfer funds between accounts. It integrates **Amazon Lex** for chatbot interactions, **AWS Lambda** for backend logic, and **AWS CloudFormation** for automated infrastructure deployment.

## Features

- **Account Balance Inquiry**: Users can check their balance by specifying an account type and confirming their date of birth.
- **Fund Transfers**: Securely transfer funds between accounts with user confirmation.
- **Confirmation Prompts**: Ensures secure transactions with user consent before completing transfers.
- **Context Management**: Enables session data carryover to enhance follow-up interactions, preventing users from re-entering data.

## Tools and Services Used

- **Amazon Lex**: For chatbot interactions.
- **AWS Lambda**: Executes backend logic and generates random account balance data.
- **AWS CloudFormation**: Automates the deployment and management of the chatbot infrastructure.
- **Amazon S3**: Used for storing additional project resources.

## Key Insights

- Successfully integrated **context carryover** to streamline user interactions.
- Implemented **confirmation prompts** for secure and verified fund transfers.
- Resolved **Lambda and Lex permission** issues that occurred during testing.
- Deployed infrastructure efficiently using **CloudFormation**.

## How It Works

1. Users initiate a request for balance inquiry or fund transfers through the chatbot.
2. **Amazon Lex** processes the request and triggers **AWS Lambda** for backend processing.
3. **Lambda** calculates the account balance or processes the transfer request.
4. The chatbot prompts the user for confirmation before finalizing the transaction.

## Documentation:
You can view the full project documentation, including all visualizations and analysis, in this [PDF](https://gabrielmazer.github.io/AWS-Projects/AWS_ChatBot.pdf).