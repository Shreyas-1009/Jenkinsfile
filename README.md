# jenkinsfile
code for checking devlopment,staging,production
pipeline {
    agent any

    stages {
        stage('devlopment') {
            steps {
                echo 'I am in devlopment stage'
                sh 'docker --version'
            }
        }
                stage('Staging') {
            steps {
                echo 'I am in Staging stage'
                sh 'git --version'
            }
        }
                stage('Production ') {
            steps {
                echo 'I am in Production stage'
                sh 'python --version'
            }
        }
    }
}

Build Now CONSOLE OUTPUT

Started by user Shreyas Dixit
[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins in /var/lib/jenkins/workspace/docker
[Pipeline] {
[Pipeline] stage
[Pipeline] { (devlopment)
[Pipeline] echo
I am in devlopment stage
[Pipeline] sh
+ docker --version
Docker version 25.0.5, build 5dc9bcc
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Staging)
[Pipeline] echo
I am in Staging stage
[Pipeline] sh
+ git --version
git version 2.40.1
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Production )
[Pipeline] echo
I am in Production stage
[Pipeline] sh
+ python --version
Python 3.9.20
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
Finished: SUCCESS
.
CODE RUN SUCCESSFULLY

