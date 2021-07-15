node{
  stage('SCM Checkout'){
	def JAVA_HOME = tool name: 'Java-jdk-1.8', type: 'jdk'
     git 'https://github.com/oferwess/my-app/'
  }
  stage('Compile-Package'){
	def mvnHOME = tool name: 'maven-3.8.1', type: 'maven'
    sh "${mvnHOME}/bin/mvn package"
  }
}
