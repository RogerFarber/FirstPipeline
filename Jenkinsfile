pipeline {
   agent any

   tools {
      // Install the Maven version configured as "M3" and add it to the path.
      maven "M3"
   }

   stages {
      stage('Build') {
         steps {
            // Get some code from a GitHub repository 
            git 'https://github.com/RogerFarber/simple-maven-project-with-tests.git'
            sh "mvn -Dmaven.test.failure.ignore=true clean compile"
         }
         }
      stage("Test") {
          steps {
<<<<<<< HEAD
            git 'https://github.com/RogerFarber/FirstPipeline.git'  
=======
            git 'https://github.com/RogerFarber/simple-maven-project-with-tests.git'  
>>>>>>> 8481da678e550204d8ec32cf075a7e0ce83b9204
            sh "mvn -Dmaven.test.failure.ignore=true clean test"
            
          }

      }
      stage("Deploy") {
          steps {
<<<<<<< HEAD
            git 'https://github.com/RogerFarber/FirstPipeline.git'  
=======
            git 'https://github.com/RogerFarber/simple-maven-project-with-tests.git'  
>>>>>>> 8481da678e550204d8ec32cf075a7e0ce83b9204
            sh "mvn -Dmaven.test.failure.ignore=true clean install"
            
          }
          post {
              success {
                  archiveArtifacts 'target/*.jar'
              }

          }


      }

      }
   }
