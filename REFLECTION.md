# Reflection – Week 5 CI/CD Project

## 1. What did you learn about CI/CD this week?
- I learned the difference between Continuous Integration (CI) and Continuous Deployment (CD).  
- CI ensures code is tested, validated, and built automatically on every push or pull request.  
- CD extends CI to deliver or deploy code into environments (staging/production).  
- I practiced GitHub Actions workflows with matrix builds, artifacts, and Slack notifications.

## 2. What challenges did you face in the pipeline?
- Initially, the working-directory paths were incorrect, causing jobs to fail.  
- Slack notifications did not trigger until the secret was properly added in GitHub.  
- Copying files between repositories created missing files until `.gitignore` was configured properly.  
- Debugging failed jobs in GitHub Actions required learning how to read logs carefully.

## 3. How would you improve your current pipeline for a production-grade project?
- Add caching for dependencies (Node modules) to reduce build times.  
- Include linting and formatting tools (ESLint, Prettier) to enforce code quality.  
- Add security checks (npm audit, dependency scanning).  
- Deploy artifacts automatically to a cloud service (e.g., AWS, Netlify, or Vercel).  
- Configure branch protection so that code must pass CI/CD checks before being merged.

