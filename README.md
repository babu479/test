# test

kubectl run -i --tty load-generator --image=busybox /bin/sh

Hit enter for command prompt

while true; do wget -q -O- http://guestbook.mstakx.io; done


 kops create cluster --master-count=1  --master-size=t2.micro --node-count=2 --node-size=t2.medium --zones=us-east-1a --name=divinu.co.in --state=s3://kops-ext-ip123 --yes
 
 kops delete cluster divinu.co.in --state=s3://kops-ext-ip123 --yes
