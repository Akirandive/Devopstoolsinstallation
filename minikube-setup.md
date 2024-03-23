Minikube installation 

Required machine config: T2.medium machine.

-minikube required service account .

step1 - launch machine with t2.medium .


step2 - install docker with root user. 
   
      >>yum install docker -y
       
      >> syatemctl start docker
      >> systemctl enable docker
     
      >>cat /etc/groups  ----> showing docker group
 
     >> user add velocity
     >> passwd velocity 
  
     >> visudo      --give all root access
 
     >> gpasswd -a velocity docker ------give access to velocity 



step 3: install kubectl in docker ----Client -command line for 

      -curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
   
       >> kubectl version
       >> kubecl  version --client

step 4: install minikube in machine

        curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64

        >> minikube start 




                         
