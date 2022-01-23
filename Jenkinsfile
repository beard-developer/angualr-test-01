node {
  stage('Checkout SCM') {
    git branch: 'main', url: 'https://github.com/beard-developer/angualr-test-01.git'
  }

  stage('Install node modules') {
    bat "yarn install"
  }

  stage('Build') {
    bat "yarn build:prod"
  }
}
