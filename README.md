Step 1:
To start the process, run pb-new-vpc-bastion.yaml. This file creates the vpc and the bastion host.

Step 2:
Capture the value for the VPCID and the public subnets from the output stream.

Step 3:
Update the pb-new-vpc-bastion-eks.yaml with the values captured in step 2.

Step 4:
Update .taskcat.yml by replacing the bastion yaml file with the eks yaml file.

5Step 5:
Run taskcat!

Note: The goal is to progressively apply each yaml file which has the next stack configuration setting. As you step through the files you will see previous stacks have been removed by adding a comment to each line in the respective stacks.