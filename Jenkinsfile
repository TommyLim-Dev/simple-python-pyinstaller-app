pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                    sh 'git init'
                    sh 'cd /var/jenkins_home/workspace/submission-cicd-pipeline-tommy/simple-python-pyinstaller-app/'
                    sh 'git pull https://github.com/TommyLim-Dev/simple-python-pyinstaller-app master'
            }
        }
        stage('Test') {
            steps {
                sh 'python3 /var/jenkins_home/workspace/submission-cicd-pipeline-tommy/simple-python-pyinstaller-app/sources/test_calc.py'
            }
        }
    }
}
