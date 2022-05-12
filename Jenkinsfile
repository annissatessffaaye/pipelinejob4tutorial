pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Crush-Steelpunch/Jenkins-Easy-Runstage.git'
            }
        }
        stage('Run') {
            steps {
                sh 'sh ./myscript'
            }
	}
        stage('Archive') {
            steps {
                archiveArtifacts artifacts: 'output', followSymlinks: false
            }
        }
    }   

}
