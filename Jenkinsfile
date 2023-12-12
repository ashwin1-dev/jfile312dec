pipeline {
  agent any

  tools {
     maven "jenkin-maven"
      }


   stages {
         stage('scm') {
              steps {
                      git 'https://github.com/ashwin1-dev/12-dec-23-war.git'
                    }
                   }

         stage('build') {
	       steps {
		 sh "mvn clean package"

                   }
              }

        stage('deploy') {
              steps {
                 sh 'echo "Deployed on system "  '
                     }
                }
    }
}

