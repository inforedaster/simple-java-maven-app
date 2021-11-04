@Library('shared-library') _

pipeline {
     agent { label 'docker-slave' }
  stages {
        stage('Git clone') {
            steps {
            sh 'git clone  https://github.com/jenkins-docs/simple-java-maven-app.git .'
                  }
            }
        stage('build') {
            steps {
              mvnBuildClassic()
            }
        }
    }
}
