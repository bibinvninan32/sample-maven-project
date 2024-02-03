pipeline {
  agent {
        label 'windows'  // Replace with the labell of your Windows node
    }
  stages {
  stage('Maven install') {
    steps {
      withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven3', mavenSettingsConfig: '', traceability: true) {
    bat 'mvn clean install'
}
    }
  }

}

}
