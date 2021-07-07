# cloud-formation
cloud formation for my project 



    aws cloudformation create-stack \
    	--stack-name fnol-ecs-deployment \
    	--template-body file://./fnol-ecs-api.yaml \
    	--capabilities CAPABILITY_NAMED_IAM \
    	--parameters 'ParameterKey=SubnetID,ParameterValue=subnet-c8635893'

    
    aws cloudformation delete-stack --stack-name fnol-ecs-deployment