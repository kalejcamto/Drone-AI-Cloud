# Drone-AI-Cloud
This is a Proof of Concept solution on a need of a drone business to make their drone fly with AI with EC2 from AWS

School Project - Case Study 
Cloud-Based Ecosystem for Next-Generation Defense Unmanned Aerial Vehicle (UAV) Capstone Cloud-A.I
Company Name
SeaScope Technologies
Canada

Cloud Student
carla.campos004@mymdc.net

Professor
Dr. Ernesto Lee
Github Repository
https://github.com/kiocardenas/Shark_Cloud


📋 Project Proof of Concept

Overview
In this project, we will be using machine learning to enable a drone to fly autonomously based on visual inputs. We will train a machine learning model to recognize objects and navigate the drone accordingly. The processing will be done on AWS EC2, a cloud-based virtual server.
What type of project is this? Next-Generation Defense Unmanned Aereal Vehicle (UAV) Cloud-A.I project.
What user problem is being solved managed in cloud based technology for scalability and availability.
Hypothesis
By migrating the software infrastructure to the cloud utilizing Amazon EC2 for elasticity, we hypothesize that we can significantly enhance our system's scalability and flexibility. 

We believe that leveraging EC2's ability to dynamically scale compute resources based on demand will lead to improved performance, reduced operational costs, and increased responsiveness to changing workloads. This elasticity will enable our application to seamlessly handle varying levels of traffic and workload spikes, ensuring optimal performance and user satisfaction. Additionally, we anticipate that by leveraging the cloud's infrastructure, we will be able to streamline our operations, reduce maintenance efforts, and enhance overall system reliability. Our hypothesis posits that the cloud migration, specifically utilizing EC2's auto-scaling features, will result in a more resilient, efficient, and cost-effective software solution.
Metrics

Accuracy: If the project involves a machine learning model or algorithm, accuracy measures how well the model predicts or classifies data correctly. It's a common metric in various scientific and technical domains.
Precision and Recall: These metrics are often used in fields like information retrieval and machine learning. Precision measures the accuracy of positive predictions, while recall measures the ability to find all the relevant cases in a dataset.

Throughput: In projects related to hardware or data processing, throughput measures how much data or how many tasks can be processed within a given time frame.
Response Time: For software applications, response time measures the time taken by the system to respond to a user's input. It is crucial for assessing user experience and system performance.

Cost-effectiveness: This metric evaluates how efficiently the project achieves its goals concerning the resources utilized, such as time, money, or manpower. It is vital for assessing the project's economic feasibility.

Scalability: Scalability metrics assess how well the project can handle an increasing amount of workload or data. It is crucial for evaluating the project's ability to handle growth.

User Engagement: For projects involving user interfaces or user experiences, metrics related to user engagement, such as click-through rates, user satisfaction surveys, or user retention rates, can be important.

Reliability and Availability: Metrics related to system uptime, downtime, and failure rates are essential for assessing the project's reliability and availability, especially in critical applications.

Energy Efficiency: In projects involving hardware, IoT devices, or mobile applications, metrics related to energy consumption are vital, especially for sustainable and battery-powered devices.

Compliance: For projects in regulated industries, metrics related to compliance with industry standards and regulations are crucial.

In summary, metrics in a scientific proof of concept project are quantitative or qualitative measures used to evaluate the project's performance, reliability, user experience, cost-effectiveness, and other aspects relevant to its goals. These metrics provide a basis for objective analysis and decision-making, guiding the project's development and determining its success.

Tools and Technologies
Tools and Technologies that would be used:

Drone Hardware: Information from the Unmanned Aerial Vehicle with an API for remote control.

Machine Learning Framework: Python with libraries like TensorFlow, Keras, or PyTorch for building and training your machine learning model.

Object Detection Model: Implement an object detection model, such as YOLO (You Only Look Once) or SSD (Single Shot MultiBox Detector) for real-time object recognition.

AWS Account: Sign up for an AWS account to use services like EC2, S3, and IAM (Identity and Access Management).

AWS EC2 Instance: Create an EC2 instance with GPU support to accelerate machine learning tasks.

Networking: Set up VPC (Virtual Private Cloud) and security groups to ensure secure communication between the drone and EC2 instance.

Remote Drone Control: Use a compatible communication protocol (like MAVLink) to control the drone remotely.

Data Storage: Utilize Amazon S3 to store training data, models, and other resources.

Data Labeling: Label training data for the machine learning model. You can use Amazon SageMaker Ground Truth or other labeling tools.

Monitoring and Logging: Use AWS CloudWatch for monitoring and logging to keep track of EC2 instance performance and application logs.

Region: AWS Canada (Central) Region (Montreal closer to Nova Scotia, Canada. There are five Amazon CloudFront edge locations in Vancouver, Toronto, and Montreal.


Pre-analysis
Process:
1. Setting Up AWS EC2 Instance:
Launch an EC2 instance with GPU support, ensuring it's in the same region as your drone for low latency communication.
Configure security groups to allow communication between the drone and the EC2 instance.
Install necessary libraries and dependencies for machine learning and drone communication.
2. Data Collection and Labeling:
Capture images and videos using the drone's camera.
Label the data for training the object detection model. Store the labeled data in Amazon S3.
3. Machine Learning Model Development:
Develop an object detection model using TensorFlow, Keras, or PyTorch. Train the model using the labeled data stored in S3.
Optimize the model for real-time inference and export it for deployment.
4. Drone Integration and Control:
Establish communication between the EC2 instance and the drone using MAVLink or another suitable protocol.
Implement code on the EC2 instance to receive video frames from the drone, process them using the trained model, and send control commands back to the drone for autonomous flight.
5. Testing and Iteration:
Test the autonomous flight in a controlled environment to ensure the drone responds correctly to detected objects.
Monitor system performance, making necessary adjustments to the model and control algorithms for accuracy and stability.
6. Monitoring and Optimization:
Set up AWS CloudWatch to monitor EC2 instance metrics, ensuring efficient resource utilization and performance.
Optimize the machine learning model for speed and accuracy, considering constraints like limited processing power on the drone and EC2 instance.
7. Security and Compliance:
Implement security best practices, including encryption, secure communication, and access control, to protect data and system integrity.
Ensure compliance with regulations and guidelines related to drone operation and data processing in your region.
Notes:
Regularly backup your model and data on Amazon S3 to prevent data loss.
Implement error handling and fail-safe mechanisms to handle unexpected situations, ensuring the safety of the drone and the system.
Keep security and privacy considerations at the forefront of your project, especially when dealing with images and videos captured by the drone.
EC2 would autoscale starting from a Large Compute Optimized type.
By following these steps and utilizing the mentioned tools and technologies, we can create a proof of concept for a cloud-based project to fly UAV using machine learning and AWS EC2. This is a complex project that requires careful planning, testing, and iteration to achieve a reliable and efficient autonomous flight system.

✨ Conclusions
Highlights

Primary goal
Find the right machine learning algorithm for the specific UAV to train the model correctly.
Secondary goal
Use the AWS to optimize costs. AWS provides tools like the AWS Pricing Calculator to estimate costs based on your usage patterns, which can be helpful in making an informed decision.


Takeaways

Pay-as-you-go Pricing: AWS operates on a pay-as-you-go model, where you pay for the resources you use. This can be advantageous as you can scale resources up or down based on demand, optimizing costs.

No Upfront Capital Costs: There are no large upfront capital expenditures in AWS. You don't need to invest in physical hardware.

Managed Services: AWS offers various managed services, reducing the need for in-house expertise. This can lead to cost savings on IT personnel.

Scalability: AWS provides elasticity, allowing you to scale resources dynamically. This ensures you don't over-provision, saving costs during low-demand periods.

Follow-up
Mark the stages of each process from start to deployment.
Measure up the metrics and make adjustments if necessary
