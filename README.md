# GIPlan

## Planograma visual, auditivo, fácil de implementar

![Presentando GIPlan](assets/GIPLANPortada.png)

## Overview

WorkAble AI is an intelligent platform designed to support employment coaches who work with people with disabilities. By leveraging Azure AI services, the system enhances coach productivity, streamlines administrative tasks, and improves job matching outcomes. Our solution addresses the critical challenge faced by supported employment programs: limited resources for job coaches who must simultaneously manage documentation, deliver personalized training, solve emerging problems, and provide motivational support to participants.

Through intelligent automation and AI-powered insights, WorkAble AI allows coaches to focus more on meaningful interactions with participants and less on administrative burdens, ultimately improving employment outcomes for people with disabilities.

![Workable AI Dashboard](./assets/dashboard_rounded.png)

## Key Features

- **Participant Management**: Complete profiles with skills, preferences, and employment history
- **Smart Session Management**: Schedule, record, and analyze coaching sessions
- **Intelligent Job Matching**: AI-powered recommendations based on participants' abilities and preferences
- **Coaching Insights**: AI-generated observations and action suggestions for personalized support
- **Interactive Dashboard**: Filter and sort participants by employment stage and view key statistics
- **Calendar Integration**: Coordinate and track sessions with participants

### Solution to problematics

| **Problematics**                          | **Solutions**                                                      |
| ----------------------------------------- | ------------------------------------------------------------------ |
| Struggling to manage administrative tasks | Calendar, Group of tables and forms (Sessions, Participants, Jobs) |
| Personalized support                      | Job Suggestions / AI Insights                                      |
| Real-time problem-solving                 | Job Suggestions / AI Insights                                      |

## Architecture / Tech Stack

WorkAble AI leverages multiple Azure services to deliver a comprehensive solution:

![Arquitectura GIPlan](assets/ArquitecturaGIPlan.png)

### Repo

Serves as the central code repository, housing both the frontend and backend code. Ensures version control and collaborative development workflows.

- **GitHub**: Stores and manages the codebase, issues, and pull requests.
- **Next.js / Tailwind css**: Frontend framework and library for building interactive user interfaces.
- **Flask / Python**: Backend framework and language for handling server-side logic and API routes..

### Animación

Analyzes participant profiles and job listings to provide intelligent job recommendations. Leverages AI-driven search and language models to match skills and preferences accurately.

- **Azure AI Search**: Retrieves and ranks relevant job postings based on participant data.
- **OpenAI / GPT-based Models**: Enhances job-matching logic with advanced language understanding.

### Instrucciones de audio

Transcribes and processes meeting conversations for insights and action items. Assists job coaches by generating real-time suggestions and storing key discussion points.

- **AI Speech**: Converts spoken content into text for further analysis.
- **AI Language**: Extracts entities, sentiments, and insights from transcribed text.
- **Calendar Integration**: Synchronizes meeting schedules and notifications with Microsoft Outlook.

## Responsable AI

Microsoft has established seven core principles to ensure the responsible development and deployment of AI technologies. Below is a table outlining these principles and their presence in the development of the project.

| **Principles**         | **How they are included**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fairness               | - Using objective, skills-based matching criteria without relying on Personal Identifiable Information (PII) in job suggestions<br>- Consistently applying the same job matching criteria to all participants with similar qualifications and needs<br>- Evaluating compatibility based on relevant factors like skills, accommodations needed, transportation status, and employment goals—not personal characteristics<br>- Maintaining balance between participant needs and job requirements without favoring certain groups                                                                                                                                                                                                        |
| Inclusiveness          | - Designed to support people with disabilities in finding and retaining meaningful employment<br>- Promotes social inclusion by helping job coaches focus on empowering participants through AI-assisted insights<br>- Considers accessibility features, supportive environments, and accommodation availability in job matches                                                                                                                                                                                                                                                                                                                                                                                                         |
| Reliability and Safety | - Analyzing multiple dimensions of compatibility (skills, accommodations, location, schedule, etc.) for robust matching<br>- Presenting job compatibility reasons that coaches can verify and validate<br>- Leaving final match decisions to human coaches who understand nuanced participant needs<br>- Maintaining structured data schemas that ensure consistent evaluation criteria<br>- Supporting coaches with clear visualizations and organized information to prevent oversight of critical factors<br>- Providing tools for ongoing session tracking and participant progress monitoring to ensure continuous support                                                                                                         |
| Transparency           | - Clearly displaying compatibility reasons for each job match, helping coaches understand why specific recommendations were made<br>- Showing match scores based on objective criteria from participant and job profiles<br>- Providing detailed job information and participant requirements side-by-side for transparent comparison<br>- Enabling coaches to see which specific factors (like required skills, accessibility features, accommodations) contributed to match recommendations<br>- Offering visibility into the matching process through detailed views that expose the reasoning behind AI suggestions<br>- Supporting coach decision-making with clear information presentation rather than black-box recommendations |
| Privacy and Security   | - Not using Personal Identification Information in the job matching algorithms<br>- Implementing strict access controls where only authorized coaches can access their participants' personal information<br>- Using secure database partitioning with appropriate keys (as shown in the Cosmos DB container configuration)<br>- Storing sensitive data in compliance with data protection regulations<br>- Separating personal identifiers from matching criteria to maintain privacy during job suggestions<br>- Ensuring that participant data is well-protected and safely stored in secure cloud infrastructure<br>- Maintaining appropriate data boundaries between different user roles in the system                            |
| Accountability         | - Humans remain in control<br>- Provides intelligent job suggestions, but the final decisions are always made by the job coach<br>- Ensures human oversight and ethical decision-making throughout the process                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 
## Development

### Project Structure

```
OXXO-Challenge/
├── README.md
└── my-app/
    ├── .gitignore
    ├── Generar Estante Bien.ipynb
    ├── next.config.ts
    ├── package.json
    ├── postcss.config.mjs
    ├── README.md
    ├── requirements.txt
    ├── tsconfig.json
    ├── xd.py
    ├── xd2.py
    ├── public/
    │   ├── Oxxo_Logo.svg
    │   ├── Planograma_bueno.csv
    │   ├── planograma_layout.json
    │   ├── Planogramas/
    │   │   ├── Estante_1.png
    │   │   ├── Estante_2.png
    │   │   ├── goodtexture.jpg
    │   │   └── plastic.jpg
    │   └── Product images/
    │       ├── Archivos de imagenes
    └── src/
        └── app/
            ├── favicon.ico
            ├── globals.css
            ├── layout.tsx
            └── page.tsx
```

### Key Components

- **Participant Dashboard**: View and manage participant information
- **Session Management**: Record and analyze coaching sessions
- **Job Listing**: Browse and assign job opportunities
- **Calendar View**: Manage upcoming sessions and availability

## Future Enhancements

- **Voice Transcription**: Automatic transcription and analysis of coaching sessions
- **Mobile Application**: Enable on-the-go access for job coaches working in the field
- **Advanced Analytics**: Deeper insights into coaching effectiveness and outcomes
- **Expanded Job Sources**: Integration with additional job boards and employment databases
- **Family Portal**: Secure access for families to view progress and contribute information

## Technology Stack

- **Frontend**: Next.js, TypeScript, Fluent UI React components
- **Backend**: Node.js, Express
- **AI**: Azure OpenAI

## License

This project is licensed under the MIT License - see the LICENSE file for details.
