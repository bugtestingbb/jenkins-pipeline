pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh('zap.sh -cmd -quickurl http://example.com -quickprogress -quickout ${WORKSPACE}/zap_report.html')
				archiveArtifacts artifacts: 'zap_report.html'
            }
        }
    }
}
