# status-dashboard

Go + React application using **raw CloudFormation**.

## Structure
- `backend/` — Go Chi API
- `frontend/` — React (Vite)
- `infra/` — CloudFormation template
- `buildspec.yml` — CodeBuild example

## Deploy
```bash
aws cloudformation deploy \
  --template-file infra/template.yaml \
  --stack-name status-dashboard-dev \
  --capabilities CAPABILITY_IAM
```
