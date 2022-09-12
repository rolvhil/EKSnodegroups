Template for creating a self managed EKS nodegroup with
- Instance store as root storage ephemeral0
- No EBS volume attached
- with VPC CNI plugin
- with Multus 7 additional Interface

Additional details on Instance store please read
- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html
- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/device_naming.html?icmpid=docs_ec2_console
- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ComponentsAMIs.html#storage-for-the-root-device


Using CodePipeline: https://github.com/rolvhil/CodePipeline/blob/main/selfmanaged-nodegroup-pipeline.yaml
- The parameters section on the Cloudformation template are parametized with into json files. One for test and for prod. Compress all files into .zip and upload to S3 bucket of the Pipeline

If you plan to use only the Cloudformation yaml file. Please adjust the Paramter section.