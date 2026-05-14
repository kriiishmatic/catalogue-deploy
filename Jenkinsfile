@Library('jenkins-shared-library-NJP') _

properties([
  parameters([
    string(name: 'appVersion', defaultValue: ''),
    string(name: 'deploy_to', defaultValue: 'dev')
  ])
])

def configMap = [
    project: "stackly",
    component: "catalogue",
    appVersion: (params.appVersion),
    deploy_to: (params.deploy_to)
]

EKSDeploy(configMap)