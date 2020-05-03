pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-west-2') {
                    s3Upload(file:'index.html', bucket:'mystaticbucket-0503', path:'index.html')
                }
            }
        }
    }
}