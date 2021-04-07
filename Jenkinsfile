@Library('jenkins-sample-lib')_

node('gradle') {
    stage('version') {
        version(
            "mvn"
        )
    }
    stage('checkout') {
            gitCheckout(
            branch: "master",
            url: "https://github.com/terekhovav88/SimpleSpring.git"
        )
    }
    stage('maven build') {
        sh 'sh \'mvn -B -DskipTests clean package\''
    }
}
