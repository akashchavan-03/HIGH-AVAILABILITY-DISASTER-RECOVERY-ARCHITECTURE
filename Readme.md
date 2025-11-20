AWS HIGH AVAILABILITY & DISASTER RECOVERY ARCHITECTURE
=

High Availability & Disaster Recovery Architecture with ELB Failover Simulation on AWS

PROJECT OVERVIEW
=
This project demonstrates a High Availability (HA) and Disaster Recovery (DR) setup on AWS using a multi-region architecture The goal was to ensure that the application remains available even if one AWS region fails.

AWS SERVICES USED
=
EC2– Web servers deployed in multiple regions

Elastic Load Balancer (ELB)– Distributes incoming traffic

Auto Scaling Group (ASG)– Maintains instance health and scalability

Route 53– DNS failover and health checks

ARCHITECTURE SUMMARY
=
Two EC2 instances are hosted in Region A and Region B, each with its own Elastic Load Balancer (ELB). Route 53 monitors the health of Region A and manages DNS failover, ensuring that if Region A fails, traffic is automatically redirected to Region B, maintaining high availability and disaster recovery.

ARCHITECTURE DIAGRAMS / SCREENSHOTS
=
High Availability & Disaster Recovery setup
=
<img width="997" height="747" alt="image" src="https://github.com/user-attachments/assets/4b105de6-24fd-49d9-b189-843f99a9a20e" />

OUTCOME / RESULTS
=
zero Downtime: The application remained available even when Region A was intentionally taken offline.

Automatic Failover: Route 53 DNS failover successfully redirected traffic to Region B without manual intervention.

High Availability: Multi-region EC2 setup with ELB and ASG ensured continuous service availability.

Scalability: Auto Scaling Groups allowed the architecture to handle varying loads efficiently.

Disaster Recovery: Demonstrated an effective strategy for disaster recovery across regions, minimizing business impact.
