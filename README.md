# Alfred Email Processor

The Alfred Email Processor is an intelligent email management system designed to classify and process emails efficiently. It uses a state graph to determine whether an email is spam or legitimate, drafts responses for legitimate emails, and notifies the user with a prepared draft.

## Features

- **Spam Detection**: Identifies spam emails and moves them to the spam folder with a reason.
- **Email Categorization**: Classifies legitimate emails into categories like inquiry, complaint, or thank you.
- **Response Drafting**: Automatically drafts professional responses for legitimate emails.
- **User Notification**: Notifies the user with the email details and the drafted response.

## Workflow

Below is the workflow of the email processing system:
![image](https://github.com/user-attachments/assets/94b744b0-b17e-4548-a1c5-9241a799acc9)
![image](https://github.com/user-attachments/assets/69b89e80-3105-4f9a-b98c-196b92b43efe)





## How to Run

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Set up the environment variables in the .env file:
    ```bash
    LANGFUSE_PUBLIC_KEY=your_public_key
    LANGFUSE_SECRET_KEY=your_secret_key
    LANGFUSE_HOST=https://cloud.langfuse.com
    OPENAI_API_KEY=your_open_ai_key
3. Run the Script:
    ```bash
    python main.py
    ```

## Example
- **Legitimate Email**: The system categorizes the email, drafts a response, and notifies the user.
- **Spam Email**: The system marks the email as spam and moves it to the spam folder.

## Dependencies
- `langgraph`
- `langchain-openai`
- `dotenv`
- `langfuse`
