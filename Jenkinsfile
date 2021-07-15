node{
tools {
    jdk 'Java-jdk-1.8'
  }	
  stage('SCM Checkout'){
     git 'https://github.com/oferwess/my-app/'
  }
  stage('Compile-Package'){
	def mvnHOME = tool name: 'maven-3.8.1', type: 'maven'
    sh "${mvnHOME}/bin/mvn package"
  }
}
