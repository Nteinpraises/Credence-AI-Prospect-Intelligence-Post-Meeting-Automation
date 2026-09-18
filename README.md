# Credence AI Prospect Intelligence & Post-Meeting Automation 
is an n8n-based automation system designed to help Credence research prospects before meetings and turn meeting information into clear recommendations and personalized follow-ups after meetings. The system combines public web research, AI analysis, Google Docs, and email notifications to reduce manual research and follow-up work while keeping the process simple and human-controlled.

# Workflow 1: Pre-Meeting Prospect Intelligence

The first workflow starts when a prospect submits a form with information such as their name, email, company, job title, website, LinkedIn profile, meeting reason, meeting date, and additional context. n8n normalizes the information, performs research using publicly available sources, and collects relevant information about the prospect and company.

The research looks for useful signals such as growth, pain, transition, engagement, and other relevant business activity. The collected information is then analyzed by AI using the SEE → LOCK → OFFER methodology. The AI identifies specific observations, possible gaps or opportunities, and useful areas for discussion while clearly separating facts from assumptions.

The workflow then creates a Google Doc containing a structured Prospect Brief with the prospect overview, public positioning, relevant signals, SEE → LOCK analysis, discussion opportunities, suggested questions, cautions, and sources. The document is stored in a dedicated Google Drive folder, and Blossom receives a notification with the prospect information and document link.

# Workflow 2: Post-Meeting Analysis

The second workflow begins after the meeting. Instead of changing the original Prospect Brief, Blossom creates a separate Meeting Review Google Doc containing the prospect information, meeting transcript or notes, and her own review. The document is placed in a dedicated Meeting Reviews folder.

n8n detects the new Meeting Review and uses the Prospect ID, email, or name and company to find the matching original Prospect Brief. It then provides both documents to AI for comparison.

The AI identifies what was confirmed during the meeting, what changed from the original research, the prospect's actual problems and goals, new information, opportunities, and remaining uncertainties. It then applies the SEE → LOCK → OFFER methodology to generate a specific recommendation and the appropriate next step.

Finally, n8n creates a Post-Meeting Analysis Google Doc containing the analysis, recommendation, and personalized follow-up message. Blossom is notified by email and receives the recommendation, next step, follow-up message, and link to the complete analysis.

# Technology

Built with n8n, AI/LLMs, public web research, Google Drive, Google Docs, and email automation.

# Purpose

The project demonstrates how AI and workflow automation connects prospect research, meeting intelligence, analysis, recommendations, and follow-up into one structured process, reducing repetitive manual work while preserving human review and decision-making.
