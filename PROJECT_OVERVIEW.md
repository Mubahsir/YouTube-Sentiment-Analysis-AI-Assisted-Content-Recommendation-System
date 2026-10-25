# Project Overview

## Aim
Analyze public YouTube comments related to a Pakistani brand and produce evidence-based content recommendations.

## Research questions
1. What is the distribution of positive, neutral, and negative sentiment in collected comments?
2. How do title-keyword content categories compare on likes and comment counts?
3. Which categories have the highest positive and negative comment shares?
4. What cautious, data-derived content tests can be recommended?

## Workflow
1. Search for videos using the YouTube Data API.
2. Collect available top-level public comments and video statistics.
3. Clean empty, duplicate, and emoji-only comments.
4. Score comments with a pretrained multilingual sentiment model.
5. Categorize videos with transparent title-keyword rules.
6. Summarize results, chart trends, and generate recommendations.
7. Export CSV, Excel, PNG charts, metadata, and Markdown report.

## Key limitations
- YouTube API quota limits and disabled comments can reduce the sample.
- Search results may include unofficial or irrelevant channels; review video results before interpreting them.
- The pretrained model is not specialized for Pakistani brands and may struggle with Roman Urdu, sarcasm, and mixed-language comments.
- Title-based categories are approximate.
- Engagement is observational; the project cannot prove that a category caused higher engagement.
- The notebook does not collect Facebook or Instagram data.

## Suggested quality checks
- Manually label a random sample of 100–200 comments and compare with model labels.
- Report precision/recall or a confusion matrix if a human-labeled validation set is prepared.
- Review the video list and category assignments before writing conclusions.
- Include collection date, search query, model name, sample size, and limitations in the final report.
