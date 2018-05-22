node{
    stage('get from github') {
    // some block
    git changelog: false, poll: false, url: 'https://github.com/sanjaysureshmv/openmrs-core.git'
    }
    stage('build the project'){
        sh 'mvn clean install'

    }
    stag('show artifacts'){
        archiveArtifacts 'webapp/target/openmrs.war'
    }

}
