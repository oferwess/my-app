node{
    stage('SCM Checkout'){
      git 'https://github.com/oferwess/my-app/'
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
