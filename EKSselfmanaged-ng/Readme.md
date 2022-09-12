Template for creating a self managed EKS nodegroup with
- EBS volume attached
- with VPC CNI plugin
- with Multus, 7 additional Interface

Using CodePipeline: https://github.com/rolvhil/CodePipeline/blob/main/selfmanaged-nodegroup-pipeline.yaml
- The parameters section on the Cloudformation template are parametized as json files. One for test and for prod. Compress all files into .zip, name it as selfmanaged-nodegroup.zip and upload to S3 bucket - pipeline-bucket-selfmanaged-nodegroup - of the Pipeline

If you plan to use only the Cloudformation yaml file. Please adjust the Parameter section.