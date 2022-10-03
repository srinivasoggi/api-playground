pipeline {
    agent any

    stages {
        stage('installing modules') {
            steps {
               npm install
	       echo 'installing npm modules'
            }
        }
        stage('build') {
            steps {
                echo 'builing package'
		tar czf nanogram-$BUILD_BUMBER.tar.gz *
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
