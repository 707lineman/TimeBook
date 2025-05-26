
# TimeBook

TimeBook is a crew timekeeping web app for internal use. This project is built as a static frontend ready for AWS Amplify deployment.

## 🔧 Features

- Modal login screen
- Sidebar navigation
- Responsive layout with gradient background
- Custom branding
- AWS Amplify-compatible deployment

## 📁 Folder Structure

```
timebook/
├── public/
│   └── index.html
└── README.md
```

## 🚀 Deploy on AWS Amplify

1. Push this repo to GitHub
2. In AWS Amplify, choose “Host web app” → GitHub
3. Select this repo and the main branch
4. Use the following `amplify.yml` config:

```yaml
version: 1
frontend:
  phases:
    build:
      commands: []
  artifacts:
    baseDirectory: public
    files:
      - '**/*'
  cache:
    paths: []
```

5. Save & deploy – updates will sync with every commit to `main`.

## 🛠 Customize

Update branding, login logic, or expand with backend integration as needed.

---

**License:** Internal Use Only
