pipeline{
	agent any
	
	/*environment {
		NAME = 'DXC'
		COUNTRY = 'INDIA'
		STATE = 'KA'
		
		secrets = credentials('SECRET_TEXT')
	
	}*/
	
	stages{

		stage('Test'){
			steps{
				echo 'Testing..'
			}
		}
	
		//stage('Build'){
			//steps{
			
				//bat 'echo My secret is  %secrets%'
			
				//bat 'echo I work for %NAME% in %STATE% , %COUNTRY%'
				//echo 'building..'
				/*bat 'echo %date% -- %time%'
				bat """
					echo "we can do more stuff here as it as a multi steps job"
					dir 
				"""
				*/
				/*retry(3){
				
					bat 'echo hello'
				}
				
				timeout(time:3,unit:'SECONDS'){
					bat 'timeout /t 5'
				}*/
			//}
		//}
		
		/*stage('Test'){
			steps{
				echo 'Testing..'
			}
		}
		
		stage('Deploy'){
			steps{
				echo 'Deploy..'
			}
		}*/
	}
	
	post{
	
		always {
			bat 'echo I will always get executed'
		}

		success {
			bat 'echo I will always get executed when the job is success'
		}	
		
		failure {
			bat 'echo I will always get executed when the job is failed'
		}
		
		unstable {
			bat 'echo I will always get executed when the job is unstable'
		}
	}
}
