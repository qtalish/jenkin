pipeline{

  agent {

        label 'TestNode'
    
}

   
stages {

      stage('Email Notification') {

         steps {

            echo 'email'
emailext body: readFile("jenkins-mail.html"), mimeType: 'text/html', recipientProviders: [developers()], subject: 'Jenkins Mail Doc ', to: 'talish.kazi@neebal.com'       
            
	}
         
}
      
      stage('Confirm Stage') {

         steps {

            echo 'done'
         
        }
      
     }

  }

}
