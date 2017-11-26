pipeline {
    agent any
    stages {
        stage('checkout') {
            dir('build-stream-tree-plugin') {
               git url: 'https://github.com/or-shachar/build-stream-tree-plugin.git'
            }
        }
        stage('echo') {
             steps {
                sh 'cat build-stream-tree-plugin/pom.xml'
            }
        }
    }
}
