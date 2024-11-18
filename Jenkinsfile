pipeline {
    agent any
    stages {
        stage ('GetProject') {
            steps {
                git 'https://github.com/mbennett7UG/untitled.git'


            }
        }
        stage ('build') {
            steps {
                sh 'mvn clean:clean'
                sh 'mvn dependency:copy-dependencies'
                sh 'mvn compiler:compile'
            }
        }

}
}