node{
   stage('SCM Checkout'){
     git 'https://github.com/javahometech/my-app'
   }
   stage('Compile-Package'){
      // Get maven home path
      def mvnHome =  tool name: 'Maven3', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }
}
