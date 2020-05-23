pipeline {
    agent any
    stages {
stage('scm') {
steps {
    git 'https://github.com/BHARATHK22/MavenTestDemo.git'
    }
}
    stage('build') {
    steps {
        withMaven(maven : 'mymaven'){
        bat "mvn clean install"
    }
    }
}
    
   
}
}
