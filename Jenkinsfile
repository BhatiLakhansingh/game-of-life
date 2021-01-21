pipeline{
	agent any
	parameters {
	choice(name: 'CHOICE', choices: ['master', 'sprint2',], description: 'Pick something')
	}
	stages{
	    stage('example'){
		  steps{ 
		   echo "Choice: ${params.CHOICE}"
		   }
		stage('git'){
		  steps{
			git 'https://github.com/BhatiLakhansingh/game-of-life.git'
			}
		}
		stage('build'){
		   steps{
			sh 'mvn package'
			}
		}
		  
		}
	}
}
