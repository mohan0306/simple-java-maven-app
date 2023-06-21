
currentBuild.displayName = "simple-java-maven-app-#"+currentBuild.number
pipeline{
    agent any
    
    stages {
        stage('continuous download') {
            steps {
                git 'https://github.com/mohan0306/simple-java-maven-app.git'
            }
               
        }
        stage('continuous build') {
            steps {
                sh 'mvn clean install'
            }
        }
}
   
}
