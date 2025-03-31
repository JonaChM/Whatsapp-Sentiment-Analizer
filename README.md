# Chat Sentiment Analysis

## Overview
This project analyzes the sentiment of WhatsApp chat messages using natural language processing techniques. The script extracts messages, identifies authors, and determines sentiment polarity (positive, negative, neutral) for each message.

## Features
- Extracts timestamps, authors, and messages from a WhatsApp chat export.
- Utilizes **NLTK's Vader Sentiment Analyzer** to classify message sentiment.
- Displays sentiment scores for individual messages.
- Computes overall sentiment distribution.

## Requirements
Ensure you have the following dependencies installed:

```bash
pip install pandas numpy nltk emoji matplotlib pillow tk
```

## How It Works
1. **Extracting Data:**
   - Reads a user-selected WhatsApp chat export file.
   - Parses timestamps, authors, and messages.
   
2. **Sentiment Analysis:**
   - Uses **Vader Sentiment Analyzer** to assign scores to each message.
   - Categorizes messages as **Positive, Negative, or Neutral**.
   
3. **Displaying Results:**
   - Prints the first few processed messages with their sentiment scores.
   - Summarizes overall sentiment of the conversation.

## How to Use
1. Run the script.
2. A file dialog will open to select the chat export file.
3. The script processes the file and prints sentiment scores.
4. The final sentiment of the chat is displayed with an emoji representation:
   - 😊 Positive
   - 😠 Negative
   - 🙂 Neutral

## Notes
- The script assumes WhatsApp's chat format (timestamps followed by messages).
- **Vader Sentiment Analyzer** is optimized for social media-style text.
- Supports both individual and group chat exports.

## Example Output
```shell
        Date      Time      Author   Message    Positive  Negative  Neutral
0  2024-03-30  14:20  John Doe   Hello!       0.5        0.0       0.5
1  2024-03-30  14:22  Jane Doe   This is bad  0.0        0.6       0.4

Overall Sentiment: Neutral 🙂
```

## Next Steps
- Implement visualization (word clouds, sentiment trends).
- Improve message parsing for different chat formats.
- Enhance emoji-based sentiment detection.

---

