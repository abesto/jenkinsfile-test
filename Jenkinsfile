stage 'Test stage 1'

parallel 'on-openjdk-8': {
	node ('openjdk-8') {
		sh 'java -version'
	}
}, 'on-jdk-7': {
	node ('maven-jdk-7') {
		sh 'java -version'
	}
}

stage 'ENV'
node ('openjdk-8') {
	sh 'env'
	checkout scm
	sh 'ls'
}
