pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                echo "my first jenkins job"
                sh '''
                a=5
                b=6
                c= `expr $a + $b`
                '''
                
            }
        }
    }
}