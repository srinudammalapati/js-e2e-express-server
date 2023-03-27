pipeline{
    agent {label 'SPRING'}
    stages{
        stage('vcs') {
            steps {
                git url: 'https://github.com/srinudammalapati/js-e2e-express-server.git',
                branch: 'main'
            }
        }
        stage('build the nodejs') {
            steps{
                sh 'npm install'
                sh ' npm run build'
            }
        }
    }
}