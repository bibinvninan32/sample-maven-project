pipeline {
  agent any
  stages {
    stage('Maven install windows') {
        when {
            expression {
                env.OS == 'BAT'
            }
         }
        steps {
            withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven3', mavenSettingsConfig: '', traceability: true) {
            bat 'mvn clean install'
            }
        }
    }
    stage('Maven install linux') {
        when {
            expression {
                env.OS == 'UNIX'
            }
         }
        steps {
            withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven3', mavenSettingsConfig: '', traceability: true) {
            sh 'mvn clean install'
            }
        }
    }
    }   
}
