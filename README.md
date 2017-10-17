# jupyter.notebooks
notes for different jyputer notebook


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
