# ec2-db-elb

This is a yaml file to create an ec2 instance with an internet-facing elastic load balancer and a database. 


The ec2 instance is launched with a condition to use a an existing ami(MyAMI) entered by the user in the parameters and if it does not exist or if the parameter is left blank, to use the default ami from the mappings. 

The elastic load balancer allows for http port 80 and the ec2 instance is attached to it. 

The database is launched using an existing snapshot entered by the user in the DBSnapshot parameter.

The DataBaseSubnet requires more than one subnet and should span at leas two availability zones. 



