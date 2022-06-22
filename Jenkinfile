pipeline{
    agent any
        stages{
		stage('Git Clone'){
            steps{
                git branch: 'main', url: 'https://github.com/Rameshagwd/Pipeline_Deploy.git'
            }
        }
		stage('MVN Clen'){
            steps{
                sh 'mvn clean'
            }
        }
        
        stage('Maven Compile'){
            steps{
                sh 'mvn compile'
            }
        }
		stage('Maven validate'){
            steps{
                sh 'mvn validate'
            }
        }
        stage('Maven Test'){
            steps{
                sh 'mvn test'
            }
        }   
        stage('Maven package'){
            steps{
                sh 'mvn package'
            }
        }
		stage('Maven Deploy'){
            steps{
                sh 'mvn deploy'
            }
        }
        
        
    }
}