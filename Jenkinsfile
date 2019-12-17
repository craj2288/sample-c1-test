podTemplate(containers: [
    containerTemplate(name: 'docker', image: 'docker', ttyEnabled: true, command: 'cat')
    ]) {
  node(POD_LABEL) {
    stage('Run shell') {
      container('docker') {
        sh 'echo hello world'
        sh 'docker --version'
      }
    }
  }
}
