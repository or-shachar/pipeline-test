pipeline {
    agent any
    stages {
        timestamps {
            stage('checkout') {
                steps {
                    dir('${repo_dir}') {
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
}
