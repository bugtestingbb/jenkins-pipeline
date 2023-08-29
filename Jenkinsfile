pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
		sh(wget https://github.com/zaproxy/zaproxy/releases/download/v2.11.1/ZAP_2.11.1_Linux.tar.gz
		tar -xvf ZAP_2.11.1_Linux.tar.gz
		cd ZAP_2.11.1
		./zap.sh -cmd -quickurl https://www.example.com -quickprogress -quickout ${WORKSPACE}/zap_report.html)
            }
        }
    }
}
