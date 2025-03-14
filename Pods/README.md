# LABS

1. How to create a pod with nginx image?
- kubectl run nginx --image=nginx

-----------------------------------------------

2. To check the image used to create pods?
- kubectl describe pod $NAME | grep image

![image](https://github.com/user-attachments/assets/b9b63a4e-2cce-40db-bc68-cb4cc7488cdd)

-----------------------------------------------

3. To check on which nodes the pods are placed on?
- kubectl get nodes

4. To check how many containers are in our pod?
- kubectl get pods - gives number (2/2) running

5. To check which images are used for our pod
- kubectl describe pods #name - check images section

6. To check why container is in error status
- kubectl describe pod #name
- Go to events section and check for the reason

7. RREADY option
- Running containers in pod/Total containers in POD

8. Create a new pod with the name redis and the image redis123.
- kubectl run redis --image=redis123 --dry-run=client -o yaml > redis-definition.yaml
- kubectl create -f redis-definition.yaml

9. 
