# autoscale-lambda-ec2
Simple script using python to scale / spawn &amp; respawn ec2 instance with lambda function.


I personally use this script to spawn ec2 for runner on aws integrated with eventbridge.

**How to Use**

I assume you have autoscaling group & Launch template created on aws to launch ec2 instance with your own specification.

For this script to use, you just need to add to lambda function and add env variables
DESIRED_CAPACITY for instance you want to launch (cannot less than MIN_SIZE)
MAX_SIZE for max total instance you want to launch
MIN_SIZE for min instance you want to launch (can be equal to 0)
NAMES use this variable as your autoscaling group name

