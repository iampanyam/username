node {
  wrap([$class: 'BuildUser']) {
    def user = env.BUILD_USER_ID
  }
}
pipeline {
    agent {
        label 'master'
            }
      stages {
        stage('Build') {
            steps { 
                sh'''
                 echo "Git Url: ${GIT_URL}"
                 echo "Git Commiter Name: ${GIT_COMMITTER_NAME}"
                 echo "Git Previous Commit: ${GIT_PREVIOUS_COMMIT}"
                 echo "Git Branch: ${GIT_BRANCH}"
                 echo "Git Author Name: ${GIT_AUTHOR_NAME}"
                 echo "Build No: ${BUILD_ID}"
                 echo "Job Url: ${JOB_DISPLAY_URL}"
                 echo "Job Name: ${JOB_NAME}"
                 echo "Build display name: ${BUILD_DISPLAY_NAME}"
                 echo "Build User: ${BUILD_USER}"
                 echo "Full Name: $BUILD_USER"
                 echo "User id: $BUILD_USER_ID"
                 '''
            }
        }
        
    }
    
}
