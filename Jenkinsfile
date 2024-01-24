pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                   git branch: 'main', url: 'https://github.com/Takaritchi-00/demo-counter-app-main.git'
            }
        }
        stage('UNIT testing'){
            
            steps{
                              sh 'mvn test'
            }
        }
        // stage('Integration testing'){
            
        //     steps{
                
        //         script{
                    
        //             sh 'mvn verify -DskipUnitTests'
        //         }
        //     }
        // }
        // stage('Maven build'){
            
        //     steps{
                
        //         script{
                    
        //             sh 'mvn clean install'
        //         }
        //     }
        // }
        // stage('Static code analysis'){
            
        //     steps{
                
        //         script{
                    
        //             withSonarQubeEnv(credentialsId: 'sonar-api') {
                        
        //                 sh 'mvn clean package sonar:sonar'
        //             }
        //            }
                    
        //         }
        //     }
            // stage('Quality Gate Status'){
                
            //     steps{
                    
            //         script{
                        
            //             waitForQualityGate abortPipeline: false, credentialsId: 'sonar-api'
            //         }
            //     }
            // }
        }
        
}