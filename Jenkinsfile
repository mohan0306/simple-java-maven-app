
currentBuild.displayName = "Game-of-Life-#"+currentBuild.number
pipeline{
    agent any
    
    stages {
        stage('continuous download') {
            steps {
                git 'https://github.com/mohan0306/simple-java-maven-app.git'
            }
               
        }
}
   
}
