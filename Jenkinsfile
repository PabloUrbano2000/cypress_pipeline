pipeline {

    agent any
    
    tools {nodejs "node"}
 
    stages {
 
        stage('Cypress Parallel Test Suite') {
            parallel {
                stage('Slave 1') {
                    agent {
                        label "Agente1_1"
                    }
                    steps {
                        git url: 'https://github.com/PabloUrbano2000/cypress_pipeline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run cypress run --record --key 2da95632-b4b1-4bee-9a8d-ddb356896a7f  --parallel'
                    
                    }
                }
 
                stage('Slave 2') {
                    agent {
                        label "Agente1_2"
                    }
                    steps {
                        git url: 'https://github.com/PabloUrbano2000/cypress_pipeline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run cypress run --record --key 2da95632-b4b1-4bee-9a8d-ddb356896a7f  --parallel'
                    
                    }
                }
 
                stage('Slave 3') {
                    agent {
                        label "Agente1_3"
                    }
                    steps {
                        git url: 'https://github.com/PabloUrbano2000/cypress_pipeline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run cypress run --record --key 2da95632-b4b1-4bee-9a8d-ddb356896a7f  --parallel'
                    
                    }
                }
 
                stage('Slave 4') {
                    agent {
                        label "Agente1_4"
                    }
                    steps {
                        git url: 'https://github.com/PabloUrbano2000/cypress_pipeline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run cypress run --record --key 2da95632-b4b1-4bee-9a8d-ddb356896a7f  --parallel'
                    
                    }
                }
 

            }
 
             
        }
 
    }
            
}