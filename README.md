# PhD_Candidate_assessment
Analyze a GitHub repository by selecting one predefined research question, collecting and  analyzing data, and reflecting critically on the findings — including any challenges faced and  any use of AI tools.

## RQ1: How does the number of commits change over time (monthly or weekly)?
 Extracted data like hash, Author name, author email, date, message, files, insertions, deletions, lines changed and converted as a CSV file.
Then there was a plotting line based on the number of commits per month.

##  What difficulties or errors did you face while completing this task?
During the task, I encountered a few key difficulties:
PyDriller import issue: Initially, the error cannot import name 'RepositoryMining' from 'pydriller' occurred due to version conflicts and environment issues. Reinstalling and ensuring no conflicting filenames in the directory resolved this.
Large repository: Since numpy/numpy is a large and mature repository, traversing all commits took significant time and memory. Optimizing with minimal data extraction and saving intermediate results helped.
Date parsing errors: While plotting, I had to ensure the date column was properly parsed as a datetime object to extract monthly periods.
File and modification tracking: Understanding how PyDriller handles file lists (modified_files vs modifications) required careful attention to documentation.

## Share the full conversation (ChatGPT or AI tool)
To solve this assignment, I mostly went through Stackoverflow and Chat GPT: "https://chatgpt.com/share/685d4971-4b10-800d-a81e-701061bd7c0d"

## Choose one of your plots: What do you find surprising, confusing, or ambiguous about it? What might explain this?
Plot: monthly_commit_trend.png – Monthly Commit Activity Line Plot
Observation:
There were a few sudden spikes and notable dips in monthly commit counts.
Some months had very low activity, especially in early years (likely during initial setup or low contributor count).
A sharp increase around 2020 stood out.

## What would be one interesting follow-up question or analysis to pursue based on your findings?
An interesting follow-up analysis would be:
"What file types or modules are most actively developed or refactored over time?"
This would complement RQ1 with insights into where development activity is focused.
