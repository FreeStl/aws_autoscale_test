1) Create a Launch Template. Choose OS type and instance type. It is important, that you don’t choose “Request spot instances” now
![Screenshot 2023-10-14 151447.png](lt%2FScreenshot%202023-10-14%20151447.png)
![Screenshot 2023-10-14 150740.png](lt%2FScreenshot%202023-10-14%20150740.png)
![Screenshot 2023-10-14 150720.png](lt%2FScreenshot%202023-10-14%20150720.png)

2) Create Auto Scaling group. As you can see, in autoscale group I overridden some Launch template configuration and added spot instances: 50% Spot, 50% on demand.
Of cource, you should specify Load Balancer, Security Group etc...
![Screenshot 2023-10-14 151729.png](asg%2FScreenshot%202023-10-14%20151729.png)
![Screenshot 2023-10-14 151711.png](asg%2FScreenshot%202023-10-14%20151711.png)
![Screenshot 2023-10-14 151645.png](asg%2FScreenshot%202023-10-14%20151645.png)

3) Set up scaling policy based on AVG CPU usage
![Screenshot 2023-10-14 150354.png](..%2F..%2FPictures%2Fauto%2FScreenshot%202023-10-14%20150354.png)

4) Set up scaling policy based on requests amount that allows non-linear growth 
![Screenshot 2023-10-14 150305.png](..%2F..%2FPictures%2Fauto%2FScreenshot%202023-10-14%20150305.png)

