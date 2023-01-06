pipeline {
    agent any

    stages {
        stage('Deploy Application') {
            steps {
                sshPublisher(publishers: [sshPublisherDesc(configName: 'JENKINS', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: '', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '/var/www/html/new', remoteDirectorySDF: false, removePrefix: '', sourceFiles: '\'"/\',php')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
            }
        }
    }
}
