pipeline {
  agent none
  stages {
    stage('Maven install linux') {
        agent {
                label 'linux'
            }
        steps {
            withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven3', mavenSettingsConfig: '', traceability: true) {
            sh 'mvn clean install'
            }
        }
    }
    stage('Maven install windows') {
        agent {
                label 'windows'
            }
        steps {
            withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven3', mavenSettingsConfig: '', traceability: true) {
            bat 'mvn clean install'
            }
        }
    }
    }   
}
