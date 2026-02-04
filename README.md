# FUTURE_ML_01
This project builds a resume screening system for a Registered Nurse role that cleans unstructured text, matches RN-specific skills, scores and ranks candidates, highlights missing skills, and visualizes results. It demonstrates an interpretable, recruiter-friendly approach to decision-support systems used in HR-tech and hiring platforms.
Enhancements and Explainability

To make the resume screening system more practical and recruiter-friendly, several enhancements were added on top of the basic skill-matching logic. These improvements focus on transparency, interpretability, and usability, which are critical in real-world hiring tools.

1. Missing Skill Identification

In addition to identifying the skills present in each resume, the system explicitly highlights the missing RN-required skills for every candidate.
For each resume, the matched skills are compared against the full RN skill list.
Skills that do not appear in the resume are marked as missing.
This allows recruiters to quickly understand skill gaps instead of only seeing a final score.
This feature supports informed decision-making by showing why a candidate may not be a strong fit and what skills they would need to improve.

2. Percentage-Based Scoring

Raw skill counts can be difficult to interpret, especially when comparing candidates. To address this, the system converts each candidate’s score into a percentage match.
Percentage score = (Number of matched RN skills / Total RN skills) × 100
This makes candidate comparisons more intuitive and standardized.
Recruiters can quickly understand how closely a resume matches the RN role requirements.
This mirrors how many real screening tools present candidate fit metrics.

3. Visual Candidate Ranking

A simple bar chart visualization is used to display candidate rankings based on their RN skill scores.
Each bar represents a candidate.
Taller bars indicate stronger alignment with RN requirements.

Summary:

With these enhancements, the system goes beyond basic keyword matching and becomes a transparent decision-support tool that:
Ranks candidates clearly
Explains why candidates rank higher or lower
Highlights missing skills
Presents results in both textual and visual formats
The chart provides a quick, high-level comparison of all candidates.

This visual summary is useful for non-technical stakeholders and helps communicate results clearly during reviews or presentations.

## Notebook Walkthrough

The full implementation and analysis are available in the Jupyter Notebook:
- `resume_screening_rn.ipynb`

The notebook includes data preprocessing, skill extraction, candidate scoring, ranking, and visual explanations.

## Project Structure

- resume_screening_rn.ipynb – complete implementation of resume screening, scoring, ranking, and visualization
- README.md – project overview, methodology, and explanation
- LICENSE – MIT license
- requirements.txt – list of project dependencies


## Limitations and Future Work:

Skill matching relies on explicit keyword mentions and may miss implicit skills.
Synonyms and variations are not fully captured.
Future improvements could include semantic similarity, skill weighting, and PDF resume parsing.

