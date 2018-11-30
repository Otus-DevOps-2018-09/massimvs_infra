# massimvs_infra
#massimvs Infra repository

#this works fine
# ssh -i ~/.ssh/infra -A -t massimovs@35.205.140.127 ssh 10.142.0.2

#and the solution for alias
# alias someinternalhost='ssh -i ~/.ssh/infra -A -t massimovs@35.205.104.97 ssh 10.132.0.3'
# someinternalhost
testapp_IP=35.187.99.191
testapp_port=9292


# task 
gcloud compute instances create reddit-app --boot-disk-size=10GB  --image-family ubuntu-1604-lts  --image-project=ubuntu-os-cloud  --machine-type=g1-small  --tags puma-server  --restart-on-failure --metadata-from-file startup-script=./deploy.sh


# availability
http://35.187.99.191
