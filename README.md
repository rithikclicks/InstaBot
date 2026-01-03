# InstaBot Hybrid - Backend (Termux)

This is the Python backend for the InstaBot Hybrid. It runs locally on Termux (Android) and connects to the cPanel frontend via Ngrok.

## Installation on Termux

1.  **Update Termux & Install Python/Git**:
    ```bash
    pkg update && pkg upgrade -y
    pkg install python git -y
    ```

2.  **Clone this Repository**:
    ```bash
    git clone <YOUR_GITHUB_REPO_URL>
    cd <REPO_NAME>
    ```

3.  **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Running the Bot

1.  **Start the API**:
    ```bash
    python api.py
    ```

2.  **Expose via Ngrok**:
    Open a new Termux session and run:
    ```bash
    ngrok http 5000
    ```
    *Copy the provided HTTPS URL and use it in the Web Frontend.*
