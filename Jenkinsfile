node {
    stage('Initialize') {
        env.PYTHONPATH="tests"
        sh 'curl -L "https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose'
    }

    stage('checkout') {
        checkout scm
    }
    stage('build') {
        sh 'docker-compose -f docker-compose-jenkins.yml build'
    }
}