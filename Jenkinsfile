pipeline {
  agent {
     node { label 'workstation' }
    }

   stages {

      stage('code Checkout') {
        steps {
          echo 'code checkout'
           }
      }

     
//build step no need for python

    stage('UNIT TESTS') {
        steps {
           echo 'UNIT TEST'
            }
        }

    stage('CODE ANALYSIS') {
        steps {
          echo 'sonar'
          //sh 'sonar-scanner -Dsonar.host.url=http://172.31.86.8:9000 -Dsonar.login=admin -Dsonar.password=admin321 -Dsonar.projectKey=frontend -Dsonar.qualitygate.wait=true'
           }
        }

    stage('SECURITY SCAN') {
       steps {
          echo 'SECURITY SCAN'
          }
       }
    stage('PUBLISH A ARTIFACT WITH VERSION') {
       steps {
          echo 'PUBLISH A ARTIFACT WITH VERSION'
          }
      }

   }

}


