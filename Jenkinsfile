pipeline {
  agent {
        label 'windows'  // Replace with the label of your Windows node
    }
  stages {
  stage('Maven install') {
    steps {
      withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven3', mavenSettingsConfig: '', traceability: true) {
    sh 'mvn clean install'
}
    }
  }

}

}
