pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo "build with Maven"
            }
            
        }
        stage('Integration Test'){
            steps{
                echo "Run with selenium"
            }
        }
        stage('Code Analysis'){
            steps{
                echo "analyzing, Tool is Jenkins!"
            }
        }
        stage('Security Scan'){
            steps{
                echo "Scanned, Nmap"
            }
        }
        stage('Deploy to staging'){
            steps{
                echo "Server Started. AWS EC2"
            }
        }
         stage('Integration Testints on staging'){
            steps{
                    echo "Run integration! the environment is production"
                }
            }
        stage('Deploy to production'){
            steps{
                echo "Deployment of the application to a production server"
            }
        }
		
		post{
                success{
                    mail to:"dheerajkumarchelani@gmail.com",
                    subject:"Integrated Git with Jenkins",
                    body:"Build has been done, Successfully!"
                }
            }
    }
}