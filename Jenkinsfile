pipeline{
	agent any
	stages{
		stage('git'){
			git 'https://github.com/BhatiLakhansingh/game-of-life.git'
		}
		stage('build'){
			sh 'mvn package'
		}
	}
}
