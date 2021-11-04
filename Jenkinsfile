@Library('shared-library') _

pipeline {
     agent { label 'docker-slave' }
  stages {
        stage('build') {
            steps {
              mvnBuildClassic()
            }
        }
    }
}
