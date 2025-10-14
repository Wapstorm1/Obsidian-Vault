* AWS - it is a cloud platform that provided comp resources like: servers, DBs or storage. 
  
  There are some core AWS services that are very popular:
  * **EC2** (Elastic Compute Cloud) - virtual servers in a cloud. Usually used to run test env. Also as a tester you can connect to the EC2 via [[SSH]] (to check logs, restart services, run auto scripts).
  * **S3** (Simple Storage Service) - it is a service to store files. Basically like a cloud USB flashdrive. QA can upload there a lot of test data or check them from S3. 
  * **IAM** (Identity and Access Management) - AWS security and permission system. In case of using we can highlight test env. or CI/CD and this thing controls what can you access. 
  * **Cloud Watch** - monitoring and logging system. If it is used on project all logs, errors, falling test will go there. 
  * **AWS CLI/Console** - Ways to interact with AWS. Okay so it is a way how to use AWS itself. It can be rather through an interface or using terminal. 