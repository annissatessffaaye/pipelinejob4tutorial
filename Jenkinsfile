pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/annissatessffaaye/pipelinejob4tutorial.git'
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
