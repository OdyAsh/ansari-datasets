---
mode: 'agent'
tools: ['codebase', 'editFiles', 'fetch', 'runCommands', 'runNotebooks', 'runTasks', 'search', 'searchResults', 'terminalLastCommand', 'terminalSelection', 'usages']
description: 'Convert HTML quiz questions to Markdown and CSV formats for Quran Tadabbor Wa Aamal sub-quizzes'
---

# HTML to Markdown/CSV Quiz Converter for Quran Tadabbor Wa Aamal

Your goal is to convert quiz questions from an HTML file to properly formatted Markdown and CSV files for the Quran Tadabbor Wa Aamal project.

## Requirements:

1. Automatically detect the latest HTML quiz file (quiz-X.html) in the sub-quizzes directory
2. Create or update the corresponding Markdown file (quiz-X.md) and CSV file (quiz-X.csv)
3. Format each question in Markdown with proper Arabic text and RTL support
4. Ensure each question has the following structure in the MD file (with a TOC at the top of the file):
   ```markdown
   ## سؤال X - [Question title]
   
   [Question text in Arabic]
   
   * [Option 1]
   * [Option 2]
   * [Option 3]
   * [Option 4]
   
   ## الإجابة الصحيحة
   
   * [Correct answer]
   ```
5. Format each question in the CSV file with:
   - category: "القرآن"
   - question: The complete question text
   - options: All options separated by commas
   - correct: The correct answer
6. Add a table of contents at the beginning of the MD file
7. Ensure that you write down the EXACT questions and answers in the processed html file, don't be creative.
   7.1 However, if the correct answer is more than 1 option , then and only then are you allowed to be creative by combining them into a single option, and choose that as the correct answer

## Process:

1. Find the latest quiz-X.html file in the sub-quizzes directory
2. Read the HTML file to extract all question content
3. Format the questions for both Markdown and CSV formats
4. Add the "الإجابة الصحيحة" (correct answer) section to each question in the MD file
5. Update the table of contents accordingly in the MD file
6. Create or update both the MD and CSV files

## Formatting Details:

If the Markdown file already has some questions, add only the missing ones.
Always maintain RTL formatting for Arabic text.
Ensure all text is properly encoded and displays correctly.
For the CSV file, follow the format: category,question,options,correct

Now, please find the latest HTML quiz file in the sub-quizzes directory and convert its questions to both Markdown and CSV formats.
