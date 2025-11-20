1.Amazon EC2
   =

  Web servers deployed in Region A (Primary)
 <img width="1889" height="876" alt="Screenshot 2025-11-20 110256" src="https://github.com/user-attachments/assets/5c47aa7c-5b20-44a7-887b-d8b5d6158259" />

Region B (Secondary/DR).
<img width="1881" height="864" alt="Screenshot 2025-11-20 112947" src="https://github.com/user-attachments/assets/bb3b2af2-6222-455a-a343-8d2fa715247b" />

2.Auto Scaling Group configuration
=
Region A
<img width="1892" height="409" alt="Screenshot 2025-11-20 110844" src="https://github.com/user-attachments/assets/0dabedca-7052-4ebe-8cf6-f6e018bf7365" />

Region B
<img width="1895" height="914" alt="Screenshot 2025-11-20 113342" src="https://github.com/user-attachments/assets/4ac63c75-ecba-405f-8281-c25d0e2bb082" />

3.ELASTIC LOAD BALANCER (ELB) setup
=
Region A 
<img width="1895" height="916" alt="Screenshot 2025-11-20 111520" src="https://github.com/user-attachments/assets/40ca2b34-e51b-484d-86d2-d33f74902c5d" />
Region B
<img width="1887" height="867" alt="Screenshot 2025-11-20 113833" src="https://github.com/user-attachments/assets/1b4bd340-cb85-4d4c-88ea-a2bde51947db" />

4.ROUTE 53 HEALTH CHECK & FAILOVER
=
<img width="1397" height="511" alt="Screenshot 2025-11-20 123320" src="https://github.com/user-attachments/assets/1f917d80-630e-49a0-adab-99d7f142fcac" />

application running in Region A
<img width="1602" height="213" alt="Screenshot 2025-11-20 115731" src="https://github.com/user-attachments/assets/a0886810-317b-4c8b-9e76-80d57fafe57c" />
application running in Region B after Route 53 triggered a DNS failover
