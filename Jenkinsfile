pipeline {
    agent any
    tools {
        maven 'MAVEN-HOME'
    }
    stages {
        stage('git repo & clean') {
            steps {
                bat "git clone https://github.com/ranith28/Maven-25BD5A6615.git"
                bat "mvn clean -f Maven-25BD5A6615/MavenWebProject25BD5A6615"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f Maven-25BD5A6615/MavenWebProject25BD5A6615"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f Maven-25BD5A6615/MavenWebProject25BD5A6615"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f Maven-25BD5A6615/MavenWebProject25BD5A6615"
            }
        }
    }
}
