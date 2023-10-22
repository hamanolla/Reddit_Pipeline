# Infrastructure as a Tool

We'll use an infrastructure-as-code tool called Terraform. This will allow us to quickly setup (and destroy) our AWS resources using code. <br>

Note that Terraform works with multiple cloud resources, not just AWS. <br>

We'll use Terraform to create:

1.Redshift Cluster <br>

Redshift is a columnar data warehousing solution offered by AWS. This will be the end destination for our data. <br>

2.IAM Role forRedshift <br>

Role we assign to Redshift which will give it permission to read data from S3. <br>

3.S3 Bucket <br>

Object storage for our extracted Reddit data. <br>

4.Security Group <br>

This particular security group will be applied to Redshift, and will allow all incoming traffic so our dashboard can connect to it.<br>
