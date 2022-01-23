node {
  stage('Checkout SCM') {
    git branch: 'main', url: 'https://github.com/beard-developer/angualr-test-01.git'
  }

  stage('Install node modules') {
    bat "npm install"
  }

  stage('Build') {
    bat "npm run build:prod"
  }

  stage('Deploy') {
    bat "pm2 restart all"
  }
}
