# Guide for setting up the k8s-cluster

# Prerequisites
- Get access to the evoila-Lab. Refer to the [internal Sharepoint-Site](https://evoilade.sharepoint.com/sites/intranet/knowledge/evoila-lab/SitePages/Zugang-beantragen.aspx).
- Contact the BU-Lab-Admin to get access to the [VMware Cloud Director](https://vcd.evoila-lab.work/login/?service=tenant:bu-bigdata&redirectTo=%2Ftenant%2Fbu-bigdata%2F).

# Setting up the K8s-Cluster
- Step 1: Navigate to the K8s-Cluster-Overview
![Alt-Text](screenshot/setup_k8s_step_1.jpg "Step 1")
- Step 2: If there is already a Cluster, go to Step X, otherwise, click on "NEW" to create a new cluster:
![Alt-Text](screenshot/setup_k8s_step_2.jpg "Step 2")
- Step 3: Follow the interface. Chose the following config on Step 4.
    - Stackable needs at least version `1.26` of kubernetes
![Alt-Text](screenshot/setup_k8s_step_3.jpg "Step 3")
    - Chose the needed amount of nodes. The count of the nodes can be changed later through the interface, but not the size. Chose `best-effort-medium` for a test setup and `best-effort-large` for a production setup. As a starting point, select 1 Control Plane Node and 8 Worker Nodes
    - Select the default settings for the other steps
- Step 4: Wait for the deployment. Afterwards, download the kube-config:
