# How to set up lab environment on Google

You can use either Google Colab or set up a virtual machine on Google Cloud Platform (GCP). It is receommended to use Google Colab unless you need to use GPU for long time.
## Google Colab:
Colab is a Python development environment that runs in the browser using Google Cloud. You can access it at [Google Colab website](https://colab.research.google.com).

### Requesting free GPU usage

1. Open the jupyter notebook file and click "Runtime" on the menu, and choose "Change runtime type". 
2. In the Notebook Setting box, choose "GPU" for "Hardware accelerator", and "High Ram" for "Runtime shape".

### Upgrade to Google Colab Pro

If you need priority access to faster GPUs and TPUs, sign up for [paid version for Colab](https://colab.research.google.com/signup).

## Google Cloud Platform (GCP): Setting up CPU and GPU Instances
This note provides a step by step guide on setting up a 
[Google Cloud Platform (GCP)](https://cloud.google.com) 
virtual machine (VM) instance with most of the 
tools necessary for this class.  GCP has made the process considerably
easier by using pre-built images with all the necessary software installed.

The note will cover creating both CPU and GPU isntances.
Although most labs in this class can be performed
with a CPU instance, a GPU instance is highly recommended for the deep learning lab.
You may also wish to consider using GPUs for your project, particularly if you
are training a deep network with a large number of parameters.
Using these instances
can dramatically speed up training of deep networks
and are essential for large-scale
problems.
Note that the per hour costs of GPU instances are much more expensive than
regular CPU instancess, so you want to make sure you turn off the instances
you are not using.  

### Requesting GPU quota
To use a GPU on GCP, you will need to first request GPU access.  For CPU instances, you can skip this step. When you initlialy register for GCP, you will be using the free service and you cannot request GPU quota. To request GPU, you have to upgrade your account to a paid account first.
1.  Go to the [IAM & admin page](https://console.cloud.google.com/projectselector/iam-admin)
2.  Select the project you are using or create a new one.
3.  Select "Quotas" on the left menu. 
4.  There are a large number of quotas that can be edited.  To find
    the correct quota, select on the top of the page:
    *   Service:  "Compute Engine API"
    *   Name:  "GPUs (all regions)"


    If you don't see "Compute Engine API", you can jump tp the next section and create a VM from a Google Instance. Once it is done, it will remind you to increase the quota for GPU.

5.  You will now see a list of metrics, one for each zone. Select the zone that is
    best for you.
6.  After you have selected the item, select "Edit Quotas" at the top of the page.
    You will be prompted to answer some questions on why you need the GPUs.
    Request at least one more GPU.
7.  You should hear from them quite fast (sometimes even within the same day!) 

### Creating the VM from a Google instance
The fastest way to get up and running is to use a pre-built image with all
the software installed.  The steps are as follows:
1.  Go to the [Google Deep Learning VM webpage](https://console.cloud.google.com/marketplace/details/click-to-deploy-images/deeplearning).
    Select "Launch on Compute Engine".  Select the project you want the VM associated with.    
2.  Select the parameters:
    * Deployment name:  Give this any name, say "tensorflow-gpu" or "tensorflow-cpu".
    * Zone:  If you are using a GPU,  you must select the same zone where you have the quota, say "us-east1-b".  Not all
    zones have GPUs.
    * Machine type:  2 vCPUs with 13 GB memory  
    * Check "Enable access to Jupyter Lab via URL"
    * Set Boot disk to 100 GB
    
    In addition, for GPU instances, select:
    * GPUs:  1 NVIDIA Tesla P100 
    * Check Install NVIDIA GPU driver
3.  Look at the price on the right.  Depending on the CPU/GPU/Storage requested, the price could vary greatly (Few cent to few dollars per hour) So be very careful with using these machines!*	
4.  Select "Deploy".      The VM will now take several minutes to deploy.
5.  Now go to the [instance listing page](https://console.cloud.google.com/compute/instances).
    You should see your instance and should be running.  You can connect to it via SSH
    VM by clicking the "SSH". 

### Configuring the VM
We next need to reconfigure the VM.
1.  If the instance is running, stop the VM by selecting the VM on the
    [instance listing page](https://console.cloud.google.com/compute/instances)
    and then hit "Stop".
2.  Click the name of the VM on the instance listing page.  You will be taken to a "VM 
    instance details" page.  Select "Edit".
3.  Select "Allow HTTP traffic" and "Allow HTTPS traffic".
4.  Select "allow full access to all Cloud APIs"
5.  Optionally, reserve a Static IP Address
    *	Navigate to the [Google Cloud Networking page](https://console.cloud.google.com/networking/addresses/list)
    *   Change the IP type of your VM instance to static.
    *   If you don't reserve a static IP address, you will have to enter the
        dynamic IP address each time.
6. You can start/stop your VM instances at anytime on the  [instance listing page](https://console.cloud.google.com/compute/instances). Don't forget to stop your VM when you are not using it to avoid extra fee.
        


### Access Jupyter notebook on the VM

1. Navigate to the [Google AI Platform page](https://console.cloud.google.com/ai-platform), and click "Notebooks" on the left side panel. You will see a list of VM instances that have Jupyterlabs.

2. Start the instance and click "OPEN JUPYTERLAB". 

3. [Optional] You can connect your Jupyterlab with your Github repo in the opened Jupyter notebook session.