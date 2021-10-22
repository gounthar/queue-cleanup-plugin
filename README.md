# Queue Cleanup plugin

The Queue Cleanup plugin removes stalled items waiting in the Jenkins queue.
The plugin allows an administrator to configure a queue wait timeout and item regex pattern.
All items matching *pattern* and waiting longer than *timeout* hours will be removed from the queue.

Operation of the cleanup task is logged in `org.jenkinsci.plugins.queuecleanup`. 
The task checking period can be configured using `org.jenkinsci.plugins.queuecleanup.QueueCleanup.period`(default 1 hour).