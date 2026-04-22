pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/abdulshajahan/coderef.git'
                  }
                }
        
        stage('Deploy'){
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
