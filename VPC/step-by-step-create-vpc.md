### Example how to create VPC and EC2 and give access EC2 to the internet within VPC

1. Create VPC

![img.png](img/img_3.png)

2. Create subnet. Subnet we bind to previously created VPC and bind to AZ (for example us-east-1a). Is it good practice
   to create public and private subnets for AZ <br>

2.1. create public subnet (in subnet us-east-1a) <br>
2.2. create private subnet (in subnet us-east-1a)

![img.png](img/img_4.png)

3. Then, in 'public' subnets need to enable 'Enable auto-assign public IPv4 address', it allows access to the internet.

![img.png](img/img_5.png)

![img.png](img/img_6.png)

4. Then, we need to create 'internet gateway' and attach to previously created VPC

![img.png](img/img_7.png)

![img.png](img/img_8.png)

5. Then, we need to create 'route table'. It's good to create route table for public and private subnets separate

![img.png](img/img_9.png)

5.1. Then, we need to assign subnets to this route table

![img.png](img/img_10.png)

![img.png](img/img_11.png)

5.2. Then, we need to add route to 'public route table' that allows traffic to the internet

![img.png](img/img_12.png)

![img.png](img/img_13.png)

5.3. In 'target' assign internet gateway that we previously created

![img_1.png](img/img_14.png)

6. Then, we can create EC2 instance and VPC that we created, and this EC2 will have access to the internet

![img.png](img/img_15.png)