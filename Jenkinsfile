parallel 'on-openjdk-8': {
	node ('openjdk-8') {
		stage 'Java version: OpenJDK 8'
		sh 'java -version'
	}
}, 'on-jdk-7': {
	node ('maven-jdk-7') {
		stage 'Java version: JDK 7'
		sh 'java -version'
	}
}

node ('openjdk-8') {
	stage 'ENV'
	sh 'env'
	checkout scm
	sh 'ls'
}
