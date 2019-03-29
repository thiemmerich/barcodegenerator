pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /root/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'javac barcodegenerator/BarCodeApplication/src/com/emmerich/main/Main.java' 
            }
        }
    }
}
