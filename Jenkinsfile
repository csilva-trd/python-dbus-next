// This is a Jenkins pipeline file used to perform a static code analysis.
// For the status to be visible on GitHub, you have to add "seedlabs-ateam" collaborator & add "Jenkins (Git plugin)"
// service to your git repository.


@Library('JenkinsMain@2.16.39')_

pipelinePythonSCA(
    pythonVersion: '3.7',
    installFromSetup: false,
    runUnitTests: true,
    unitTestRunner: 'dbus-run-session py.test',
    additionalAptPkgs: 'dbus-tests',
    packages: ["."],
)
