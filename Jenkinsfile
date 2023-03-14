pipeline {
    agent { label 'ubuntu' }
    stages {
        stage('vcs') {
            steps {
                git url: 'https://github.com/purna970/spc-repo.git',
                    branch: 'develop'
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
    }
} 