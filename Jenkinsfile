pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build World'
            }
        }
            stage('Test') {
            steps {
                echo 'Test app'
            }
            }
                stage('Deploy') {
            steps {
                echo 'Deploy application'
            }
                }
        }
    post {
    success {
     mail bcc: '', body: '''A Build was triggered for your job

Note: Donot Reply to this mail

Regards 
Team Alpaha''', cc: '', from: '', replyTo: '', subject: 'Pipeline ran', to: 'ameerbatcha.learnings@gmail.com'
    }
    } 
}
