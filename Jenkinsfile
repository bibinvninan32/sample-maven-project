pipeline {
  agent linux
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
