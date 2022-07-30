# aws_codedeploy_using_github

Refer first chiplunkarshubham/aws_code_deploy as this is the continuation and userdata can also be found there.

# How to fix
CodeDeploy agent was not able to receive the lifecycle event. Check the CodeDeploy agent logs on your host and make sure the agent is running and can connect to the CodeDeploy server.

# Uninstall the codedeploy-agent
sudo yum erase codedeploy-agent -y

# Remove the codedeploy-agent file from /opt directory
cd /opt

sudo rm -r codedeploy-agent/

# Install the codedeploy-agent again.
sudo ./install auto
