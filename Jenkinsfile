def username = 'Jenkins'
pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
               git 'https://github.com/gayat19/JavaProj.git'
               bat label: '', script: 'javac Employee.java'
            }
        }
        stage('Test'){
            steps{

                echo 'Hello Mr. ${username}'
                echo "I said, Hello Mr. ${username}"
            }
        }
    }
}
