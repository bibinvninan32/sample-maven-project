pipeline {
  agent any
  stages {
  stage('Maven install') {
    steps {
      withMaven(globalMavenSettingsConfig: '', jdk: '', maven: '', mavenSettingsConfig: '', traceability: true) {
    sh 'mvn clean install'
}
    }
  }

}

}
