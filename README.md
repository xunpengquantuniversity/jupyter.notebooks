# jupyter.notebooks
notes for different jyputer notebook

#### use AMI
	#security-groups: jupyterhub, matlab(we use this one here)
	aws ec2 run-instances --image-id ami-6c8b7514 --count 1 --instance-type t2.micro --key-name jaja --security-groups {security-groups} | grep InstanceId
	aws ec2 describe-instances --instance-ids {instance-id} | grep PublicIpAddress
	aws ec2 create-image --instance-id {instance you want to create} --name "TensorFlow Inception AMI" --description "This is a AMI for TensorFlow AMI"


#### jupyter hub
    AMI: ami-1f917b67

#### R notebook
    AMI: ami-59ca0c21
    instance_config = """#!/bin/bash
    sudo docker start a8ea9ae626d6
    """
#### DataSci notebook
      AMI: ami-44c1073c
      instance_config = 
      """#!/bin/bash
      sudo docker run -d -p 8888:8888 jupyter/datascience-notebook start-notebook.sh --NotebookApp.token=''	
      """

#### GAN model for Semi-Supervised learning
	AMI: ami-a6d211de
        instance_config = 
	"""#!/bin/bash
        sudo docker start a8ea9ae626d6
        """
