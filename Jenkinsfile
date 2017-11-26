pipeline {
    agent any

    options {
        disableConcurrentBuilds()
        timeout(time: 2, unit: 'HOURS')
        timestamps()
    }
    
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
                sh 'cat build-stream-tree-plugin/pom.xml'
            }
        }
    }
}
