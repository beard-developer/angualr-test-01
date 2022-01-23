node {
  stage('Checkout SCM') {
    git branch: 'main', url: 'https://github.com/beard-developer/angualr-test-01.git'
  }

  stage('Install node modules') {
    sh "yarn install"
  }

  stage('Build') {
    sh "yarn build:prod"
  }
}
