node{
    stage('SCM Checkout'){
      git 'https://github.com/oferwess/my-app/'
  }
  stage('Compile-Package'){
	def mvnHOME = tool name: 'maven-3.8.1', type: 'maven'
	def output = sh script: 'java -jar build/output/my-tool.jar', returnStdout: true
	//def JAVA_HOME = tool name: 'Java-jdk-1.8', type: 'jdk'
    sh "${mvnHOME}/bin/mvn package"
  }
}
