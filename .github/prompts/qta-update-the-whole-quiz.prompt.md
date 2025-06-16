---
mode: 'agent'
tools: ['codebase', 'editFiles', 'fetch', 'runCommands', 'runNotebooks', 'runTasks', 'search', 'searchResults', 'terminalLastCommand', 'terminalSelection', 'usages']
description: 'Update the consolidated Quran Tadabbor Wa Aamal quiz files with content from specific sub-quizzes'
---

# Quran Tadabbor Wa Aamal Quiz Consolidator

Your goal is to consolidate specific sub-quiz files into the main comprehensive quiz files for the Quran Tadabbor Wa Aamal project.

## Requirements:

1. Identify specific sub-quiz files (quiz-*.md and quiz-*.csv) based on provided numbers or the latest quiz
2. Merge their content into the main consolidated quiz files while maintaining proper structure
3. Ensure all quiz sections, questions, and answers are properly transferred
4. In other words, transfer what's exactly mentioned in quiz-*.md/csv files, do not be creative and do not change questions or answers
4. Update table of contents in the main MD file


## Process:

1. Determine which sub-quizzes to consolidate:
   - If specific quiz numbers are provided (e.g., "1, 2, 5"), use those numbers
   - If no numbers are provided, find and use the latest sub-quiz by number
2. Read the specified sub-quiz MD files from the sub-quizzes directory
3. Merge their content into the main consolidated MD file
   - Preserve all sections, questions, options, and correct answers; do not alter them and do not be creative
   - Update/create table of contents
   - If questions already exist in the main file, don't duplicate them
4. Read the corresponding sub-quiz CSV files
5. Merge their rows into the main consolidated CSV file
   - Ensure consistent column structure
   - Maintain proper CSV formatting
   - If questions already exist in the main file, don't duplicate them

## Extra Details:

- The main quiz files are located at:
  - MD file: quran-tadabbor-wa-aamal/the-whole-quiz/quran-tadabbor-wa-aamal-quiz.md
  - CSV file: quran-tadabbor-wa-aamal/the-whole-quiz/quran-tadabbor-wa-aamal-quiz.csv

Now, please consolidate the specified sub-quiz files (${input:quizNumbers}) into the main quiz files. If no quiz numbers are specified, consolidate the latest sub-quiz only.
