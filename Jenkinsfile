cat > Jenkinsfile <<'EOF'
pipeline {
  agent any
  options { timestamps() }
  stages {
    stage('Checkout') {
      steps { checkout scm }
    }
    stage('Build') {
      steps { echo 'Hello from Jenkins pipeline!' }
    }
  }
}
EOF
