mkdir jenkins-integration-test && cd $_
git init -b main
echo "# Jenkins test" > README.md
cat > Jenkinsfile <<'EOF'
pipeline {
  agent any
  stages {
    stage('Checkout'){ steps { checkout scm } }
    stage('Build'){ steps { echo 'Hello from Jenkins!' } }
  }
}
EOF
git add .
git commit -m "Initial commit with Jenkinsfile"
git remote add origin https://github.com/<your-username>/jenkins-integration-test.git
git push -u origin main
