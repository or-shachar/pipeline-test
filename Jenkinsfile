pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                dir('${repo_dir}') {
                    git url: '${repo_url}'
               }
            }
        }
        stage('echo') {
             steps {
                sh 'cat ${repo_dir}/pom.xml'
            }
        }
    }
}
