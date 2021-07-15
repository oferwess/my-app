node{
  stage('SCM Checkout'){
     git 'https://github.com/oferwess/my-app/'
  }
  stage('Compile-Package'){
	def mvnHOME = tool name: 'maven-3.8.1', type: 'maven'
    sh "${mvnHOME}/bin/mvn package"
  }
  stage ('Email Notification'){
	mail bcc: '', body: 'test1', cc: '', from: '', replyTo: '', subject: 'my-app deploy', to: 'oferw3412@gmail.com'
	}
}
