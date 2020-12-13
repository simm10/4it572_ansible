# 4it572_ansible

	1. root/ansible
		a. mkdir group-vars
		b. mkdir group-vars/all
		c. ansible-vault create group_vars/all/aws.yml
			i. AWS account details
				1) access_key
				2) secret_key
				3) session_token
			ii. escape + :wq + enter (closes editor)
		d. ansible-playbook ec2_deploy.yml --ask-vault-pass (ec2_deploy.yml is template in the folder
