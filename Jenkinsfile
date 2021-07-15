node{
    stage('SCM Checkout'){
      git 'https://github.com/oferwess/my-app/'branch: "${params.branch}"
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
