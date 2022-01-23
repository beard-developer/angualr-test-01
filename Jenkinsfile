node {
  stage('Checkout SCM') {
    git branch: 'SP2', url: 'https://github.com/beard-developer/angualr-test-01.git'
  }

  stage('Install node modules') {
    sh "npm install"
  }

  stage('Build') {
    sh "npm build"
  }

  stage('Deploy') {
    sh "pm2 restart all"
  }
}
