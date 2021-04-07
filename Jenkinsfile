@Library('jenkins-sample-lib')_

node('gradle') {
    stage('version') {
        version(
            "mvn"
            )
    }
    stage('maven build') {
        sh 'sh \'mvn -B -DskipTests clean package\''
        }
}
