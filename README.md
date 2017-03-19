# sample_pipelines

1. Fork https://github.com/shippableSamples/sample_pipelines
1. Create a cluster on ECS named `test-cluster`
1. Enable the project from the UI in CI section
1. Navigate to Pipelines v2 page (super user)
1. Select `github` account integration
1. Select your forked `sample_pipelines` project
1. Select branch `master`

This triggers a flow that spans across `rSync`, `versionTrigger`, `stepExec (manifestSteps)` and `stepExec (ecsDeploySteps)`. You can check out the logs of these services.
