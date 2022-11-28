# staticProvisioningOfpvc
Static provisioning of PVC in eks
Before running the pv-pvc.yaml file, We need to create a volume in the AWS you can use the Console for this or you can use the below mentioned command.

`aws ec2 create-volume --availability-zone=us-west-2c --size=100 --volume-type=gp2`

After executing this command you will get the volume ID copy that and paste that in pv-pvc.yaml file. Now your pv-pvc is ready to created.

Also add the same zone in pv in which you have created the volume.
