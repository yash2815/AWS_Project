Here are the step-by-step instructions for the entire CloudWatch alerting and monitoring project I followed:

I began by logging into the AWS Management Console using my credentials.
In the console, I searched for "CloudWatch" and selected it from the services available.
I navigated to the "Metrics" section in CloudWatch to view the available metrics.
Under "Metrics," I selected EC2 and then Per-Instance Metrics to find the CPUUtilization metric for the Stress Test EC2 instance.
Next, I created a CloudWatch alarm by choosing the "Alarms" dropdown in CloudWatch and selecting "Create alarm."
For the alarm configuration, I set up the condition that triggers the alarm when the CPUUtilization exceeds 60 percent for the Stress Test EC2 instance.
I linked this alarm to the SNS topic created earlier, specifically "MyCwAlarm," to receive email notifications.
After creating the alarm, I accessed the Stress Test EC2 instance and initiated a command that stressed the CPU to 100 percent.
While the CPU was under stress, I monitored the CloudWatch Alarms page in the console for the alarm status to change to "In alarm."
Upon reaching the "In alarm" state, I confirmed the spike in CPU utilization by observing the CloudWatch graph.
Finally, I received an email notification via Amazon SNS alerting me about the In alarm state.

For detailed Instructions, check out Stepwise guide in the repository.
For visualized or pictorial guide, check out Screenshots repository
