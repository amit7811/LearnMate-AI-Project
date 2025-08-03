# LearnMate-AI-Project
IBM AI &amp; Cloud Internship Final Project – Agentic AI for Personalized Course Pathways
# LearnMate – Agentic AI for Personalized Course Pathways

![LearnMate Banner](https://img.shields.io/badge/IBM%20AI%20%26%20Cloud-Internship%20Project-blue?style=for-the-badge&logo=ibm)
![Python](https://img.shields.io/badge/Python-3.8+-green?style=flat-square&logo=python)
![IBM Watson](https://img.shields.io/badge/IBM-Watsonx-darkblue?style=flat-square&logo=ibm)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter)

## 🎯 Project Overview

**LearnMate** is an intelligent Agentic AI coach designed to revolutionize personalized learning experiences. Built as part of the IBM AI & Cloud Internship program conducted by Edunet Foundation in collaboration with IBM SkillBuild and AICTE, this project addresses the critical challenge of students struggling to identify optimal learning paths in today's overwhelming digital education landscape.

### 🔍 Problem Statement
Students often face decision paralysis when choosing from thousands of online courses across domains like Frontend Development, Cybersecurity, UI/UX Design, and more. Without personalized guidance, learners frequently:
- Select inappropriate courses for their skill level
- Follow non-optimal learning sequences
- Lack adaptive feedback mechanisms
- Miss opportunities for skill progression

**LearnMate** solves this by acting as an intelligent AI coach that understands individual learning preferences, assesses current capabilities, and dynamically constructs personalized course roadmaps that evolve with the learner's progress.

## 🛠️ Technology Stack

### Core IBM Technologies
- **IBM Watsonx AI Studio**: Primary AI development platform
- **IBM Granite Foundation Models**: Large language model for natural language understanding
- **Watsonx Runtime**: AI model deployment and inference
- **IBM Cloud Lite Services**: Cloud infrastructure and storage

### Supporting Technologies
- **Python 3.8+**: Primary programming language
- **Pandas & NumPy**: Data manipulation and analysis
- **Jupyter Notebooks**: Interactive development environment
- **LangChain**: AI agent framework integration
- **Matplotlib/Seaborn**: Data visualization
- **Streamlit**: Web application framework (bonus feature)

## 📊 Dataset Structure

### 1. User Profiles (`user_profiles.csv`)
```
UserID   | Name    | Interest                  | SkillLevel        | Goal
1        | Amit    | Frontend Development      | Intermediate      | Become React Developer
2        | Sneha   | Cybersecurity             | Beginner          | Ethical Hacking Career
3        | Ravi    | UI/UX Design              | Beginner          | Build Portfolio
```

**Features:**
- **UserID**: Unique identifier for each learner
- **Name**: Student name for personalization
- **Interest**: Primary domain of interest
- **SkillLevel**: Current proficiency (Beginner/Intermediate/Advanced)
- **Goal**: Long-term career objective

### 2. Course Catalog (`course_data.csv`)
```
CourseID | Title | Domain | Level | Platform | Duration(hrs)
101 | Intro to HTML & CSS | Frontend Development | Beginner | Coursera | 15
102 | Advanced JavaScript | Frontend Development | Intermediate | Udemy | 25
103 | Ethical Hacking Basics | Cybersecurity | Beginner | edX | 20
```

**Features:**
- **CourseID**: Unique course identifier
- **Title**: Course name and description
- **Domain**: Subject area classification
- **Level**: Difficulty tier (Beginner/Intermediate/Advanced)
- **Platform**: Learning platform provider
- **Duration**: Estimated completion time in hours

## 🏗️ AI/ML Architecture

### System Architecture Flow

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   User Input    │───▶│  IBM Granite LLM │───▶│ Intent Analysis │
│                 │    │                  │    │                 │
└─────────────────┘    └──────────────────┘    └─────────────────┘
                                                         │
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│ Adaptive        │◀───│ Course Filtering │◀───│ Skill Assessment│
│ Roadmap         │    │                  │    │                 │
└─────────────────┘    └──────────────────┘    └─────────────────┘
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│ Progress        │    │ Recommendation   │    │ Personalization │
│ Tracking        │    │ Engine           │    │ Engine          │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

### Core Components

1. **Natural Language Processing Module**
   - Powered by IBM Granite foundation models
   - Processes user queries and extracts learning intent
   - Understands context and preferences

2. **Skill Assessment Engine**
   - Evaluates current user competency
   - Maps skills to appropriate course levels
   - Identifies knowledge gaps

3. **Intelligent Recommendation System**
   - Filters courses based on user profile
   - Creates sequential learning pathways
   - Optimizes for learning efficiency

4. **Adaptive Feedback Loop**
   - Monitors user progress and completion rates
   - Dynamically adjusts recommendations
   - Implements continuous improvement

## 🚀 Deployment Plan

### Phase 1: Development & Testing
- Local development using Jupyter Notebooks
- Integration with IBM Watsonx AI Studio
- Dataset preparation and validation
- Algorithm testing and optimization

### Phase 2: Cloud Deployment
- Deploy models to Watsonx Runtime
- Configure IBM Cloud Lite services
- Implement API endpoints
- Performance monitoring setup

### Phase 3: Production & Scaling
- Web application deployment (Streamlit)
- User authentication and data security
- Real-time recommendation serving
- Analytics and feedback collection

## 📸 Output Screenshots

### 1. User Interaction Simulation

🤖 LearnMate: Hello! I'm LearnMate, your AI learning coach. 
What domain interests you most?

👤 User: I want to learn Frontend Development

🤖 LearnMate: Great choice! What's your current experience level?
[Beginner] [Intermediate] [Advanced]

👤 User: Intermediate

🤖 LearnMate: Perfect! Based on your profile, here's your personalized roadmap...
```

### 2. Adaptive Roadmap Generation

📚 Your Personalized Learning Path:

Phase 1 (Current): Advanced JavaScript (25 hrs)
Phase 2 (Next): React Fundamentals (30 hrs)  
Phase 3 (Future): Full-Stack Projects (40 hrs)

Progress: ▓▓▓░░░░░░░ 30% Complete
```

### 3. Progress Tracking Dashboard

📊 Learning Analytics:
• Courses Completed: 3/8
• Total Hours: 65/200
• Current Streak: 12 days
• Next Milestone: React Developer Certification


## 🔗 References & Resources

### IBM Documentation
- [IBM Watsonx AI Studio Guide](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/watson-machine-learning.html)
- [IBM Granite Models Documentation](https://www.ibm.com/products/watsonx-ai)
- [Watsonx Runtime Deployment](https://cloud.ibm.com/docs/watson-machine-learning)

### Tutorials & Learning Resources
- [IBM Cloud Getting Started](https://cloud.ibm.com/docs/overview)
- [LangChain Integration with IBM Models](https://python.langchain.com/docs/integrations/llms/ibm_watsonx)
- [AI Agent Development Best Practices](https://www.ibm.com/topics/ai-agents)

### Research Papers
- "Personalized Learning Path Recommendation using Deep Learning" (2023)
- "Adaptive Educational Systems: A Survey" (2024)
- "AI-Powered Career Guidance Systems" (2023)

## 🎯 Future Enhancements

### Short-term Goals
- Integration with real course platforms (Coursera, Udemy APIs)
- Mobile application development
- Multi-language support
- Enhanced UI/UX design

### Long-term Vision
- Industry partnership integrations
- AI-powered mentorship matching
- Corporate training solutions
- Advanced learning analytics

## 👨‍💻 Author
**Developed by**: Amit Prajapat
**Program**: IBM AI & Cloud Internship  
**Institution**: Edunet Foundation × IBM SkillBuild × AICTE  

## 📄 License
This project is developed as part of an educational internship program. All IBM technologies used are subject to their respective licensing terms.


*Built with using IBM Watsonx AI Studio and Granite Foundation Models*
