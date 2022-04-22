pipeline {
    agent any
    triggers {
        cron('* * * * *')
    }
    tools {
      ansible 'ansible2.12'
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                echo "my first jenkins job"
                sh '''
                a=5
                b=6
                c=`expr $a + $b`
                '''
                
            }
        }

        stage('ansibletest'){
          steps {
            sh 'ansible --version'
          }

        }
        
        stage('SAST'){
          steps {
            sh 'echo SAST'

          }

        }
    }
}