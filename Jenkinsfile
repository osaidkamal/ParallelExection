pipeline {
    agent any
    options {
        skipDefaultCheckout() }
        stages{
            
            stage("Checkout") {
                steps{
                script{
                    
                    ws("{workspace}"){
                
               steps.checkout([$class: 'GitSCM', branches: [[name: '*/${Branch}']], extensions: [], userRemoteConfigs: [[credentialsId: '2e71e8dd-67bb-4f9e-ad63-1693a71e4f3e', url: 'https://github.com/osaidkamal/ParallelExection']]])
            }
            }
                }
            }
                stage("Shell Script"){
           
            
            steps {
//             parallel(
                ws("{workspace}"){
                echo 'testing'
//                 sh 'chmod -R a+wx testing'
//                 )
                }
            }
            }
        }
}
        
