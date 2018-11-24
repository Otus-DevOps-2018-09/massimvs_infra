# massimvs_infra
massimvs Infra repository

#this works fine
ssh -i ~/.ssh/infra -A -t massimovs@35.205.140.127 ssh 10.142.0.2

#and the solution for alias
alias someinternalhost='ssh -i ~/.ssh/infra -A -t massimovs@35.205.140.127 ssh 10.142.0.2'
someinternalhost
