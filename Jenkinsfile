@Library('jenkins-sample-lib')_

node('gradle') {
    stage('version') {
        version(
            "mvn"
        )
    }
    stage('maven build') {
        withMaven() {
           git "https://github.com/terekhovav88/SimpleSpring.git"
           sh "mvn clean deploy" // 'mvnw' command (e.g. "./mvnw deploy")
        }
    }
}
