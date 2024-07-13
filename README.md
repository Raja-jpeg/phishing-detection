# phishing-detection

## To-do
- Figma design
- UI
- Machine Learning model
- Deploy

## Completed
- Figma design - draft 1


### Project Plan and Design Flow

#### Phase 1: Planning
1. **Requirements Gathering**: Define project requirements, user stories, and acceptance criteria.
2. **Technology Stack Decision**: Finalize tech stack (Python, Flask/Django, React).
3. **Architecture Design**: Choose monolithic architecture, create high-level diagrams.

#### Phase 2: Setup
1. **Project Setup**:
   - Initialize Git repository
   - Set up JIRA for project management
   - Set up Jenkins for CI/CD pipelines
2. **Environment Setup**:
   - Configure development environments for frontend, backend, and ML
   - Set up database

#### Phase 3: Development
1. **Frontend Development**:
   - Create basic React application
   - Develop UI components for URL input and results display
2. **Backend Development**:
   - Set up Flask/Django application
   - Develop API endpoints for URL submissions and results retrieval
   - Implement user authentication
3. **ML Model Development**:
   - Collect and preprocess data
   - Train and evaluate ML models
   - Integrate trained models with the backend

#### Phase 4: Integration and Testing
1. **Integrate Frontend and Backend**:
   - Connect React app with Flask/Django API
   - Ensure smooth communication between components
2. **Testing**:
   - Conduct unit tests for individual components
   - Perform integration tests to ensure end-to-end functionality
   - Conduct security testing (e.g., penetration testing)
   - Validate model accuracy and performance

#### Phase 5: Deployment and Monitoring
1. **Deploy Application**:
   - Set up production environment
   - Deploy using Jenkins CI/CD pipelines
2. **Monitor and Maintain**:
   - Monitor application performance and security
   - Gather user feedback and iterate on improvements
   - Plan for potential transition to microservices if needed

### Design Flow
1. **User Interaction Flow**:
   - User enters a URL in the frontend
   - Frontend sends URL to the backend API
   - Backend processes the URL and uses the ML model to determine if it’s a phishing URL
   - Backend sends the result back to the frontend
   - Frontend displays the result to the user

2. **Model Training Flow**:
   - Collect labeled datasets of phishing and non-phishing URLs
   - Preprocess the data (e.g., feature extraction, normalization)
   - Train and evaluate multiple ML models
   - Select the best-performing model and deploy it to the backend

3. **CI/CD Flow**:
   - Developers push code changes to the repository
   - Jenkins triggers automated tests
   - If tests pass, Jenkins deploys the new version to the production environment



### Components Required
1. **Frontend**
   - **Framework**: React
   - **Components**: User interface for URL input, results display, and user feedback
   - **State Management**: Redux or Context API for managing state

2. **Backend**
   - **Framework**: Flask or Django
   - **Components**: 
     - API endpoints for receiving URL submissions
     - User authentication and session management
     - Integration with ML models for URL analysis

3. **Machine Learning**
   - **Language**: Python
   - **Libraries**: scikit-learn, TensorFlow/PyTorch, pandas, numpy
   - **Components**: 
     - Data preprocessing pipelines
     - Model training scripts (supervised learning with labeled phishing and non-phishing URLs)
     - Model evaluation and tuning
     - Model deployment (possibly using Flask/Django or a separate service)

4. **Database**
   - **Type**: SQL (PostgreSQL/MySQL) or NoSQL (MongoDB)
   - **Components**: Storage for user data, URL submissions, and model results

5. **Project Management**
   - **Tool**: JIRA
   - **Components**: Task tracking, sprint planning, backlog management

6. **CI/CD**
   - **Tool**: Jenkins
   - **Components**: Automated testing, deployment pipelines

7. **Testing**
   - **Types**: Unit tests, integration tests, end-to-end tests
   - **Tools**: pytest (for Python), Jest (for React), Selenium (for automated UI testing)
   - **Focus**: Model accuracy, application security, performance testing




