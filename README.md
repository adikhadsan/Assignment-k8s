Kubernetes Cluster Architecture and Deployment

Description:

1. Created Docker file for Application
2. Run standalsone container using docker commands
3. created single Master and 2 worker node cluster of kubernetes
4. configured CNI callico network
5. Application yml manifest is in Application folder
6. Horizontal and Vertical pod autoscalling yml is provided in Scalling folder. metrics server is configured in cluster and vpa components are installed,
7. Config maps are used in monitoring section
8. secret were used for storing aws credential using CLI kubectl create secret generic aws-secret --namespace kube-system --from-literal "key_id=##" --from-literal "access_key=***"
9. Static storage provision and Dynamic Storage provision on AWS ebs using ebs.csi drvier is in storage folder
10. Role based Access provided in RBAC
11. Network policy created for controlling communication of pods
12. Rolling update and rollback are done using following cammands,version 2 of application were created:kubectl set image deployment demo-deploy demo-app=aditya7133/demo-app:v2 --record and kubectl rollout undo deployment demo-deploy --to-revision=3
13. Monitoring of Cluster using node exporter of prometheus and created Alert for down target which was configured in monitoring and Alert section
14. Centralized logging system created using EFK stack. yml provided in logging section 


