node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/zashraj/apigee_pipeline.git'
             
      //mvnHome = tool 'M3'
   }
   stage('Build') {
         sh "mvn -f HelloWorld/pom.xml clean install -Ptest -Dapigee.config.options=create"
   }
}
