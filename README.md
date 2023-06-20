# Helm-Chart
Learnt how to create a helm chart


To create a new Helm chart, you use: 
"helm create <chart name>"


The Different Directories and what they do:

chart.yaml: This is where you'll put the information related to your chart. That includes the chart version, name, and description so you can find it if you publish it on an open repository. 

values.yaml: , this is the file that contains the variables you would reference.
templates : This is the place where you'll put all your manifest files. Everything in here will be passed on and created in Kubernetes.
charts: If your chart depends on another chart you own, or if you don't want to rely on Helm's default library (the default registry where Helm pull charts from), you can bring this same structure inside this directory. 


To template the helm chart and ensure:
"Helm template -f <value.yaml> /the directory ((.) if you are in the current directory)


