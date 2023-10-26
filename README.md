# D-ID Video Creation and Download Script

This Python script allows you to create D-ID videos and download them using D-ID's API. You can provide a CSV file with questions, where each question has a custom filename based on job titles and question numbers.

## Prerequisites

Before running the script, make sure you have the following:

- Python installed on your system.
- Required Python packages: requests and csv (you can install them using pip).

## Usage

1. Clone or download this repository to your local machine.

2. Add your D-ID API key:

   In the script, replace `'YOUR_API_KEY'` with your actual D-ID API key.

3. Prepare your CSV file:

   Create a CSV file with the following headers:

   - "Job title": Job title for the question.
   - "Questions": The actual questions you want to create videos for.
   - "Q no": Question number (for custom filenames).

   Example CSV structure:

   ```csv
   Job title,Questions,Q no
   Engineer,Can you describe a situation where you faced a significant challenge?,1
   Designer,How do you approach design problems?,2
   ```

Run the script:

Open your terminal or command prompt and navigate to the directory containing the script and your CSV file.

Run the script using the command: python main.py
Wait for video creation and downloading:

The script will create D-ID videos for each question in the CSV file. It will wait for a short time and then download the videos.

Custom filenames:

The videos will be downloaded with custom filenames based on "Job title" and "Q no" from your CSV file.

Downloaded videos:

The downloaded videos will be saved in the same directory as the script.

Note
Make sure your API key is properly configured and has the necessary permissions.

The script includes a delay and attempts to check for the result URL. You can adjust the delay and attempts as needed.

This script provides a basic example. You can further customize it to suit your specific requirements.

For more details on the D-ID API and its capabilities, refer to the official D-ID API documentation.

License
This project is licensed under the MIT License. See the LICENSE file for details.
