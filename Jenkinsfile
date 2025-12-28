@Library('Jenkins-Shared-Library-04') _

def config = [
    // Project Variables
    PROJECT_NAME: "expense",   // required     
    PROJECT_KEY: "expense",    // required
    COMPONENT: "backend",      // required

    // Git Variables
    EXECUTE_GITCHECKOUT_STAGE: "yes",
    MY_GIT_URL: "https://github.com/vaheedgithubac/Image-Update-Check.git", // required
    MY_GIT_REPO_TYPE: "public",   // required (public/private)
    MY_GIT_CREDENTIALS_ID: "",    // required for private repos
    MY_GIT_BRANCH: "",            // Defaults to "main" if not set

    // Update Image Tag in GitHub
    EXECUTE_UPDATE_IMAGE_TAG_GITHUB_STAGE: "yes",
    DOCKER_IMAGE: "expense-backend:abcd123",
    GIT_DEPLOY_HTTPS_CREDS: "git-deploy-https-creds",
    GIT_REPO_NAME: "Image-Update-Check",
    VERSION_CONTROL_SYSTEM: "github",          // required (github/gitlab)  Defaults to 'github'
    //HELM_VALUES_FILE: "helm/values.yml" ,      // required if you want to update helm values file
    DEPLOYMENT_FILE: "kubernetes/deployment-svc.yml"                        // required if you want to update deployment file
  ]

PIPELINE_NODEJS(config)
