node{
    stage('SCM Checkout'){
      git 'https://github.com/oferwess/my-app/'
  }
  stage('Compile-Package'){
	def mvnHOME = tool name: 'maven-3.8.1', type: 'maven'
	def JAVA_HOME = /usr/lib/jvm/java-11-openjdk-11.0.11.0.9-2.el8_4.x86_64  
    sh "${mvnHOME}/bin/mvn package"
  }
}
