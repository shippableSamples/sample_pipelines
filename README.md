# sample_pipelines

i. Make sure your subscription has the `isNewPipeline: true`  
ii. Sync your account (this is required to update gitlab with your subId)  
iii. Fork https://github.com/shippableSamples/sample_pipelines  
iv. Create a cluster on ECS named `test-cluster`  
iv. Enable the project from the UI in CI section  
iv. Navigate to Pipelines v2 page (super user)  
v. Select `github` account integration  
vi. Select your forked `sample_pipelines` project  
vii. Select branch `master`  

This triggers a flow that spans across `rSync`, `versionTrigger`, `stepExec (manifestSteps)` and `stepExec (ecsDeploySteps)`. You can check out the logs of these services.  

