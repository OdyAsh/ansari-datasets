---
mode: 'agent'
tools: ['read_file', 'insert_edit_into_file', 'replace_string_in_file', 'file_search', 'list_dir']
description: 'Generate quiz questions from Quran book content for Tadabbor Wa Aamal sub-quizzes'
---

# Quiz Generator from Book Content for Quran Tadabbor Wa Aamal

Your goal is to generate multiple-choice questions based on content from Islamic book paragraphs for the Quran Tadabbor Wa Aamal project.

## Requirements:

1. Automatically detect the latest book content file (book-content-X.md) in the sub-quizzes directory
2. Create or update the corresponding quiz files (quiz-X.md and quiz-X.csv)
3. Generate 10 well-formulated multiple-choice questions in Arabic (or less, if the number of paragraphs in book-content-X.md is a small number)
4. Create a new quiz section in the MD file with an appropriate title
5. Ensure each question follows this structure in the MD file:
   ```markdown
   ## سؤال X - [Question title]
   
   [Question text in Arabic, referencing Quranic concepts from the content]
   
   * [Option 1]
   * [Option 2]
   * [Option 3]
   * [Option 4]
   
   ## الإجابة الصحيحة
   
   * [Correct option repeated here]
   ```
6. Format each question in the CSV file with:
   - category: "القرآن"
   - question: The complete question text
   - options: All options separated by commas
   - correct: The correct answer
7. Randomize the order of options so the correct answer isn't always first
8. Add a table of contents at the beginning of the MD file

## Process:

1. Find the latest book-content-X.md file in the sub-quizzes directory
2. Read and understand the book content paragraphs
3. Identify key concepts, teachings, and Quranic references
4. Create thought-provoking questions that test comprehension of the material
5. Format the questions for both Markdown and CSV formats
6. Ensure each question has exactly 4 options with only one correct answer
7. Create or update both the MD and CSV files (quiz-X.md and quiz-X.csv)

## Instructions:

- Use consistent formatting throughout
- Include Quranic verses when appropriate
- Make questions educational and thought-provoking
- Ensure questions test understanding rather than mere memorization
- Use category "القرآن" for all questions in the CSV file
- Format options in CSV with proper single quotes and commas
- Always maintain RTL formatting for Arabic text
- Ensure all text is properly encoded and displays correctly

Now, please find the latest book content file in the sub-quizzes directory and generate quiz questions based on its content.
