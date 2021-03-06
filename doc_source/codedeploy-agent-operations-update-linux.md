--------

 The procedures in this guide support the new console design\. If you choose to use the older version of the console, you will find many of the concepts and basic procedures in this guide still apply\. To access help in the new console, choose the information icon\. 

--------

# Update the AWS CodeDeploy Agent on Amazon Linux or RHEL<a name="codedeploy-agent-operations-update-linux"></a>

After the AWS CodeDeploy agent \(`codedeploy-agent.noarch.rpm`\) is installed on an instance, it is updated within 24 hours of the release of a new version\. The update time cannot be easily cancelled or rescheduled\. If a deployment is in progress during the update, the current deployment lifecycle event finishes first\. After the update is complete, the deployment resumes with the next deployment lifecycle event\.

If you want to force an update of the AWS CodeDeploy agent, sign in to the instance, and run the following command:

```
sudo /opt/codedeploy-agent/bin/install auto
```