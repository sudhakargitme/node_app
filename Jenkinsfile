pipleline {
    agent any

    stage('Clone repository') {
        /* Pull the source code from Git Hub */

        git 'https://github.com/sudhakargitme/finalproject01.git'
    }

    stage('Build image') 
{
        
    

        dockerFingerprintFrom dockerfile: 'Dockerfile', image: 'npmimg02'
    }

    stage('Test image') {
        /* Check the npm version */

        steps {
            sh 'npm --version'
        }
    }

}
