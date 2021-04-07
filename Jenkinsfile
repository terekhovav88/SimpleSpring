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
            cred: "f8413abe-394d-4162-98d5-842a7e37942d",
            url: "https://github.com/terekhovav88/SimpleSpring.git"
        )
    }
    stage('maven build') {
        sh 'sh \'mvn -B -DskipTests clean package\''
    }
}
