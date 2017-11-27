pipeline {
    agent any
    options {
      timestamps()   
    }
    stages {
        stage('checkout') {
            steps { 
                dir("${repo_dir}"){
                    git "${repo_url}"
                }
            }
        }
        stage('build'){
            steps {
                dir("${repo_dir}"){
                    sh "cat pom.xml"
                }
            }
        }
    }
}
