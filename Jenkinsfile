pipeline{
	agent any
	parameters {
	choice(name: 'CHOICE', choices: ['master', 'sprint2',], description: 'Pick something')
	}
	stages{
		stage('git'){
		  steps{
			git 'https://github.com/BhatiLakhansingh/game-of-life.git'
			}
		}
		stage('build'){
		   steps{
			sh 'mvn package'
			}
		stage('parameters'){
		  steps{ 
		   echo "Choice: ${params.CHOICE}"
		   }
		}
		  
		}
	}
}
