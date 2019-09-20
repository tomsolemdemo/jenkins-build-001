node {
        
        checkout([
                    $class: 'GitSCM',
                    branches: scm.branches,
                    doGenerateSubmoduleConfigurations: false,
                    extensions: scm.extensions + [[$class: 'SubmoduleOption', disableSubmodules: false, recursiveSubmodules: true, reference: '', trackingSubmodules: false]],
                    submoduleCfg: [],
                    userRemoteConfigs: scm.userRemoteConfigs])

    
        stage('Build') {
            echo 'Building using trackingSubmodules' 
            sh "ls -R"
        }
        stage('Test'){
            echo 'Testing....'
        }
        stage('Deploy dev'){
            echo 'Deploy dev'
        }
        stage('Deploy prod'){
            echo 'Deploy prod'
        }
    
}