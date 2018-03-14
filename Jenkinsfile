node {
    def mvnHome
    stage ('codecheckout'){
        git 'https://github.com/iqram007/course.git'
        mvnHome = tool'MAVEN_HOME'
        
    }
    stage ('compilethecode')
    sh "'${mvnHome}/bin/mvn'  clean compile"
    stage ('package')
    sh "'${mvnHome}/bin/mvn'  clean package"
    stage ('result')
    echo "successful"
}
