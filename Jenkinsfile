pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                dir('${repo_dir}') {
                    deleteDir
                    git url: '${repo_url}'
               }
            }
        }
        stage('echo') {
             steps {
                sh 'cat build-stream-tree-plugin/pom.xml'
            }
        }
    }
}
