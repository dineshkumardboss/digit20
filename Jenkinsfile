node{
    stage("git checkout"){
        git credentialsId: 'GIT_CRE', url: 'https://github.com/dineshkumardboss/digit20.git'
    }
    stage("mavn build"){
        def mvnhome = tool name: 'maven3.6', type: 'maven'
        sh"${mvnhome}/bin/mvn clean package"
    }
}
