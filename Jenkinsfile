node {
        
        checkout scm: [
                        $class: 'GitSCM',
                        branches: scm.branches,
                        doGenerateSubmoduleConfigurations: false,
                        extensions: [[$class: 'SubmoduleOption',
                                      disableSubmodules: false,
                                      parentCredentials: false,
                                      recursiveSubmodules: true,
                                      reference: '',
                                      trackingSubmodules: false]],
                        submoduleCfg: [],
                        userRemoteConfigs: scm.userRemoteConfigs
                ]

    
        stage('Build') {
            echo 'Building scm array' 
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