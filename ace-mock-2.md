# <p align="right">**Mock Test 2 – Answers**</p>

1.  Your team of developers received their own Google Cloud Project to
    use as their sandbox environment. You would like to be notified if
    any developers exceed \$1000 per month of Google Cloud spending.
    What should you do?<br><br>

<ol type="A">
<li>Set up individual billing accounts for each developer and
        manually check their monthly spending.</li>
<li>Ask the developers to report their monthly Google Cloud spending
        to you.</li>
<li>Set up a budget alert in Google Cloud that notifies you if any
        individual developer exceeds $1000 per month of Google Cloud
        spending.</li>
<li>Monitor the spending every quarter and meet with the developers
        to discuss their usage.</li>
</ol> 

<br>

<ins>Correct Answer: C</ins>

This is the most efficient and scalable way to monitor developers'
spending.

You can create a budget for each developer's project and set up alerts
to notify you when the budget is exceeded. This will allow you to
identify overspending developers and take corrective action quickly.

Here are some useful links:
- How to set up budget alerts in Google Cloud:
  <https://cloud.google.com/billing/docs/how-to/budgets>
- Managing budgets and alerts in Google Cloud:
  <https://cloud.google.com/billing/docs/how-to/budgets>
- Best practices for managing Google Cloud costs:
<https://cloud.google.com/blog/topics/cost-management/best-practices-for-optimizing-your-cloud-costs>

##

2.  Employees in a single physical location use your internal facing
    application exclusively. It requires strong consistency, fast
    queries, and multi-table ACID transactional updates. It is based on
    PostgreSQL, and you received a requirement to deploy it in Google
    Cloud with minimal code changes. Which database solution is most
    suitable for this?<br><br>

<ol type="A">
<li>Google Cloud Spanner.</li>
<li>Google Cloud SQL for PostgreSQL.</li>
<li>Google Cloud Firestore.</li>
<li>Google Cloud Bigtable.</li>
</ol>

<br>

<ins>Correct Answer: B</ins>

Google Cloud SQL for PostgreSQL is a fully managed relational database
service that makes it easy to set up, maintain, and scale PostgreSQL
databases in the cloud. It is compatible with PostgreSQL so that you can
migrate your existing PostgreSQL database to Google Cloud SQL with
minimal code changes.

Google Cloud SQL for PostgreSQL offers strong consistency, fast queries,
and multi-table ACID transactional updates. It is also highly scalable
and reliable, making it ideal for mission-critical applications.

Here are some useful links:
- Google Cloud SQL for PostgreSQL documentation:
  <https://cloud.google.com/sql/docs/postgres>
- Google Cloud SQL for PostgreSQL best practices:
  <https://cloud.google.com/sql/docs/postgres/best-practices>

##

3.  Which Google Cloud product is best suited for storing sensor data
    from construction equipment with high data throughput, consistent
    time-based data retrieval, and atomic storing and retrieving
    signals?<br><br>


<ol type="A">
<li>Google Cloud Spanner.</li>
<li>Google Cloud SQL for PostgreSQL.</li>
<li>Google Cloud Storage.</li>
<li>Google Cloud Bigtable.</li>
</ol> 

<br>

<ins>Correct Answer: D</ins>

The best Google Cloud product for storing sensor data from construction
equipment with high data throughput, consistent time-based data
retrieval, and atomic storing and retrieving signals is Google Cloud
Bigtable.

Google Cloud Bigtable is a fully managed, NoSQL database service that
offers scalability, performance, and availability for large-scale,
mission-critical applications. Bigtable is designed to handle high data
throughput and low latency reads and writes, and it can be scaled to
handle petabytes of data.

Bigtable is also a good choice for storing sensor data because it
supports atomic transactions, meaning multiple reads and writes to the
same data can be performed safely and consistently. This is important
for applications that ensure that sensor data is always accurate and
up-to-date.

Here are some useful links: 
- Google Cloud Bigtable documentation:
  <https://cloud.google.com/bigtable>

##

4.  Which of the following Google Cloud Compute Engine features can
    prevent the accidental deletion of a VM?<br><br>

<ol type="A">
<li><b>Deletion protection</b>: This feature prevents a VM from being
        deleted unless the user explicitly confirms the deletion.</li>
<li><b>Snapshots</b>: Snapshots are point-in-time copies of a VM. They
        can be used to restore a VM to a previous state if it is
        accidentally deleted.</li>
<li><b>Backups</b>: Backups are copies of a VM that are stored
        off-site. They can be used to restore a VM to a previous state
        if it is accidentally deleted or if the underlying hardware
        fails.</li>
<li><b>IAM permissions</b>: IAM permissions can be used to control who
        has access to delete a VM. This can help to prevent accidental
        deletions by unauthorized users.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

The Google Cloud Compute Engine feature that can prevent the accidental
deletion of a virtual machine is IAM permissions configuration with
delete protection.

IAM permissions configuration with delete protection allows you to
configure permissions for your Compute Engine resources to prevent them
from being deleted accidentally. To do this, you can set the
compute.instances.delete permission to Deny for any users or roles that
you do not want to be able to delete your virtual machines.

Here are some useful links:

- Google Cloud IAM Overview <https://cloud.google.com/iam>
- Configuring IAM Policies for Compute Engine
  <https://cloud.google.com/compute/docs/access/iam>
- Preventing Accidental Deletion of Resources
  <https://cloud.google.com/compute/docs/instances/preventing-accidental-vm-deletion>

##

5.  What is the first step to take when preparing to create a Google
    Cloud Spanner instance for a new project that will be used to deploy
    a globally distributed application?<br><br>

<ol type="A">
<li>Set up a Cloud Storage bucket to store backups.</li>
<li>Install the Cloud Spanner client libraries on your local
        machine.</li>
<li>Configure a firewall to allow access to the Cloud Spanner
        instance.</li>
<li>Create a Google Cloud Spanner instance configuration and select
        a multi-region or regional instance.</li>
</ol>

<br>

<ins>Correct Answer: D</ins>

The first step to take when preparing to create a Google Cloud Spanner
instance for a new project that will be used to deploy a globally
distributed application is to create a Google Cloud Spanner instance
configuration and select a multi-region or regional instance.

This is because the instance configuration determines the number of
nodes, storage capacity, and other settings for your Cloud Spanner
instance. You also need to decide whether you want a multi-region or
regional instance. Multi-region instances are more expensive, but they
offer better performance and availability.

Here are some useful links:

- Google Cloud Spanner documentation:
  <https://cloud.google.com/spanner/docs>
- Google Cloud Spanner best practices:
  <https://cloud.google.com/spanner/docs/best-practices>
- Google Cloud Spanner tutorials:
  <https://cloud.google.com/spanner/docs/tutorials>

##

6.  When configuring a VPC firewall for an application, how should you
    limit data egress to the fewest open ports?<br><br>

<ol type="A">
<li>Set up a default deny egress rule, and then create allow rules
        only for necessary ports and destinations.</li>
<li>Configure an allowlist of allowed egress IP addresses and ports.</li>
<li>Use a proxy server to restrict outbound traffic to approved
        destinations.</li>
<li>Use Cloud Audit Logging to monitor egress traffic and block any
        suspicious activity.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

The best way to limit data egress to the fewest open ports is to set up
a default deny egress rule and then create allow rules only for
necessary ports and destinations.

This approach is most secure because it blocks all egress traffic by
default and only allows traffic to specific ports and explicitly allowed
destinations. This helps to prevent unauthorised access to your data and
applications.

Here are some useful links:

- Creating VPC firewall rules:
  <https://cloud.google.com/firewall/docs/firewalls#creating_firewall_rules>

##

7.  Which steps should you take to ensure that future CLI commands, by
    default, address the specific GKE cluster named <code>development</code>?<br><br>

<ol type="A">
<li>Run the following command - <code>gcloud config set container/cluster development</code>.</li>
<li>Run the following command - <code>gcloud config set cluster/development</code>.</li>
<li>Run the following command - <code>gcloud config set container/development</code>.</li>
<li>Run the following command - <code>gcloud config set development/cluster</code>.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

To set a default cluster for gcloud commands, run the following command:
<code>gcloud config set container/cluster CLUSTER_NAME</code>

This command sets the default cluster for the gcloud CLI to
<code>development</code>, so any subsequent commands that require a cluster
reference will use this cluster by default.

Here are some useful links:

- gcloud config set
  <https://cloud.google.com/kubernetes-engine/docs/how-to/managing-clusters#default_cluster_kubectl>

##

8.  Which of the following options would be the best approach to reduce
    the cost of running a fault-tolerant batch workload that runs every
    night on many **VMs** in Google Cloud Platform?<br><br>

<ol type="A">
<li>Reduce the size of the VMs to reduce the cost.</li>
<li>Use preemptible or spot VMs to reduce cost.</li>
<li>Use standard persistent disks instead of SSD persistent disks.</li>
<li>Use larger VMs to handle the workload more efficiently.</li>
</ol>

<br>

<ins>Correct Answer: B</ins>

Preemptible VMs are short-lived VMs available at a significant discount
compared to standard VMs. They are preempted when Google needs the
resources they are using for other workloads, but they are a good option
for fault-tolerant batch workloads that can be restarted if they are
preempted.

Spot VMs are similar to preemptible VMs but are based on unused capacity
in Google's data centres. They are cheaper than preemptible VMs but more
likely to be preempted.

Here are some useful links:

- Preemptible VMs documentation (Google Cloud)
  <https://cloud.google.com/compute/docs/instances/preemptible>
- Spot VMs documentation (Google Cloud)
  <https://cloud.google.com/compute/docs/instances/spot>

##

9.  Your company operates in a strongly regulated environment. An
    auditor wants to review who accessed data in Cloud Storage buckets.
    Which options to audit access data in Google Cloud Storage buckets
    would you choose?<br><br>

<ol type="A">
<li>Use Cloud Asset Inventory to view access logs for Cloud Storage
        buckets.</li>
<li>Enable Cloud Audit Logs for Cloud Storage buckets to view
        activity logs.</li>
<li>Use the export logs API.</li>
<li>Use Cloud Storage Reports to view access logs for Cloud Storage
        buckets.</li>
</ol> 

<br>

<ins>Correct Answer: B</ins>

Cloud Audit Logs is a service that logs all administrative activity in
your Google Cloud Platform project. This includes activity on Cloud
Storage buckets, such as creating, deleting, and updating buckets and
objects.

Cloud Audit Logs complies with many industry regulations, including PCI
DSS, HIPAA, and GDPR. This makes it a good choice for auditing access
data in a strongly regulated environment.

Here are some useful links:

- Auditing access data in Cloud Storage buckets:
  <https://cloud.google.com/storage/docs/audit-logging>
- Cloud Audit Logs documentation:
  <https://cloud.google.com/logging/docs/audit>

##

10. Which of the following options would you investigate whether a
    former employee accessed sensitive customer information in Google
    Cloud after leaving the company?<br><br>

<ol type="A">
<li>Use Cloud Audit Logs to view the access history of the former
        employee's Google Cloud account.</li>
<li>Use Google Cloud DLP to scan for sensitive information in the
        Google Cloud projects and storage buckets accessed by the former
        employee.</li>
<li>Use Google Cloud's operations suite to view the former
        employee's activity logs in Google Cloud.</li>
<li>Use Cloud Identity and Access Management to check the former
        employee's access to Google Cloud and revoke it if necessary.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

Cloud Audit Logs provide a record of all activities and access events
within your Google Cloud environment, including actions taken by
specific users like former employees. This can help you track their
access and actions.

While the other options (B, C, and D) can be valuable for security and
compliance, they may not specifically address whether the former
employee accessed sensitive customer information in Google Cloud after
leaving the company.

Here are some useful links:

- Cloud Audit Logs documentation:
  <https://cloud.google.com/logging/docs/audit>

##

11. Which command can grant a user the editor role for a specific Google
    Cloud project using the gcloud command line tool?<br><br>

<ol type="A">
<li><code>gcloud projects add-iam-policy-binding</code></li>
<li><code>gcloud iam roles create</code></li>
<li><code>gcloud iam service-accounts create</code></li>
<li><code>gcloud compute firewall-rules create</code></li>
</ol>

<br>

<ins>Correct Answer: A</ins>

The command that can grant a user the <code>editor</code> role for a specific Google
Cloud project using the gcloud command line tool is: <code>gcloud projects add-iam-policy-binding</code>

This command allows you to add an IAM policy binding to a Google Cloud
project, which includes specifying the role <code>editor</code> in this case and the
user's identity.

Here are some useful links:

- gcloud projects add-iam-policy-binding:
  <https://cloud.google.com/sdk/gcloud/reference/projects/add-iam-policy-binding>

##

12. Which statement about Google Cloud VPN in **high availability (HA)**
    mode is correct?<br><br>

<ol type="A">
<li>Google Cloud VPN in HA mode is designed to provide HA by
        replicating VPN gateways across multiple regions.</li>
<li>Google Cloud VPN in HA mode is only available for use with
        Google Cloud Compute Engine instances.</li>
<li>Google Cloud VPN in HA mode is not recommended for production
        use as it can cause connectivity issues.</li>
<li>Google Cloud VPN in HA mode is a paid service that requires a
        separate subscription.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

Google Cloud VPN in HA mode is a highly available VPN solution that
replicates VPN gateways across multiple regions. This ensures that
traffic can be routed to another VPN gateway in a different region if
one VPN gateway becomes unavailable.

Google Cloud VPN in HA mode is available with Google Cloud Compute
Engine instances, other cloud providers and on-premises networks.

Google Cloud VPN in HA mode is recommended for production use and is
designed to provide reliable and consistent connectivity.

Here are some useful links:

- Cloud VPN Overview:
  <https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview>
- HA VPN topologies:
  <https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies>

##

13. Imagine that you have an application hosted on a bare-metal server
    situated in your data centre, which needs access to cloud storage.
    However, your security policies prevent the servers that host the
    application from having public IP addresses or accessing the
    internet. In such a case, you must abide by Google's recommended
    guidelines for facilitating the application's access to cloud
    storage. What actions should you take?<br><br>

<ol type="A">
<li>Use <code>nslookup</code> or <code>dig</code> command to get the IP address of
        <code>storage.googleapis.com</code>. Negotiate with the security team to
        provide public IP addresses to bare metal servers. Allow only
        egress traffic from bare-metal servers to the IP addresses of
        <code>storage.googleapis.com</code>.</li>
<li>Use Cloud VPN or Cloud Interconnect to create a tunnel to your
        VPC in Google Cloud. Use Cloud Router to create a custom route
        advertisement for <code>199.36.153.4/30</code> and <code>2600:2d00:0002:1000::/64</code>.
        Announce that network to your on-premises network through the
        VPN tunnel. In your on-premises network, configure the DNS
        server to resolve <code>*.googleapis.com</code> as a CNAME to
        <code>restricted.googleapis.com</code></li>
<li>Use Migrate for Compute Engine to migrate bare metal servers to
        Compute Engine. Create an Internal Load Balancer that uses
        <code>storage.google.com</code> as a backend. Configure new Compute Engine
        instances to use Internal Load Balancer as proxy.</li>
<li>Use Cloud VPN, create a VPN tunnel to your VPC in Google
        Cloud.  
        In the VPC, create Compute Engine with a Squid proxy. Configure
        your server to use Squid proxy to access Cloud Storage.</li>
</ol> 

<br>

<ins>Correct Answer: B</ins>

This approach sets up a secure connection between your data center and
Google Cloud using VPN or Cloud Interconnect. It also includes
configuring DNS resolution for the Google Cloud services. This allows
your bare-metal server to access Google Cloud services without exposing
it to the public internet.

Here are some useful links:

- Google Cloud VPN documentation:
  <https://cloud.google.com/network-connectivity/docs/vpn>
- Google Cloud Interconnect documentation:
  <https://cloud.google.com/network-connectivity/docs/interconnect>
- Google Cloud DNS documentation:
  <https://cloud.google.com/dns/docs>

##

14. What steps should be performed as a prerequisite before creating a
    new Compute Engine instance using the CLI, and after creating a new
    project in Google Cloud with the <code>gcloud</code> command-line tool and
    linking a billing account to the project?<br><br>

<ol type="A">
<li>Set the default project using the command <code>gcloud config set project [PROJECT_ID]</code>.</li>
<li>Enable the Compute Engine API for the project using the command
        <code>gcloud services enable compute.googleapis.com</code>.</li>
<li>Install the Google Cloud SDK on the machine where the CLI will
        be run.</li>
<li>Create a new service account with the necessary permissions to
        create Compute Engine instances.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

Before creating a new Compute Engine instance using the CLI after
creating a new project in Google Cloud with the gcloud command-line tool
and linking a billing account to the project, you should set the default
project using the command <code>gcloud config set project [PROJECT_ID]</code>.

Here are some useful links:

- Setting the default project:
  <https://cloud.google.com/sdk/gcloud/reference/config/set>

##

15. What is the command to create a new Kubernetes Engine cluster in
    Google Cloud using the <code>gcloud</code> CLI?<br><br>

<ol type="A">
<li><code>gcloud kubernetes clusters create</code></li>
<li><code>gcloud compute instances create</code></li>
<li><code>gcloud container clusters create</code></li>
<li><code>gcloud compute kubernetes create</code></li>
</ol>

<br>

<ins>Correct Answer: C</ins>

The command to create a new Kubernetes Engine cluster in Google Cloud
using the gcloud CLI is: <code>gcloud container clusters create [CLUSTER_NAME]</code>

This command will create a new Kubernetes Engine cluster in the default
zone and region. You can specify the zone and region using the <code>--zone</code>
and <code>--region</code>flags.

For example, to create a new Kubernetes Engine cluster in the
us-central1-a zone, you would use the following command: <code>gcloud
container clusters create my-cluster --zone us-central1-a</code>.

You can also specify other options for the cluster, such as the machine
type, node count, and Kubernetes version.

Here are some useful links:

- Creating a zonal cluster:
  <https://cloud.google.com/kubernetes-engine/docs/how-to/creating-a-zonal-cluster>

##

16. What steps can be taken to automate the installation of Jenkins for
    efficient and streamlined application building and deployment from
    source code during the development of a new application?<br><br>

<ol type="A">
<li>Create an instance template with Jenkins already installed.
        Create Managed Instance Group from the template.</li>
<li>Create a new Kubernetes Engine cluster and create a deployment
        from the Jenkins image.</li>
<li>Create a new Compute Engine instance and install Jenkins
        manually.</li>
<li>Deploy Jenkins from Google Cloud Marketplace.</li>
</ol>

<br>

<ins>Correct Answer: D</ins>

Google Cloud Marketplace offers pre-configured solutions, including
Jenkins, that can be easily deployed, reducing manual installation and
configuration efforts.

Here are some useful links:

- Google Cloud Marketplace: <https://cloud.google.com/marketplace>

##

17. What steps should you take to deploy additional pods that require
    **n2-highmem-32** nodes on Google Kubernetes Engine (GKE), without
    causing any downtime, given that your existing application already
    runs on multiple pods across eight GKE **n2-standard-8** nodes?<br><br>

<ol type="A">
<li>Create a new GKE cluster with <b>n2-highmem-32</b> nodes and redeploy
        the pods. After that, delete the old cluster.</li>
<li>Use the <code>gcloud container clusters upgrade</code> command and deploy new
        pods.</li>
<li>Create a new cluster with both <b>n2-highmem-32</b> and
        <b>n2-standard-8</b> nodes. Redeploy the pods and delete the old
        cluster.</li>
<li>Create a new node pool, specify the machine type of
        <b>n2-highmem-32</b> and deploy the new pods.</li>
</ol>

<br>

<ins>Correct Answer: D</ins>

Creating a new node pool with the desired machine type allows you to
scale your cluster with the specific node type required for your
additional pods without affecting the existing pods in your cluster.

Here are some useful links:

- Add and manage node pools:
  <https://cloud.google.com/kubernetes-engine/docs/how-to/node-pools>

##

18. What steps must you take to deploy a Docker image of your
    application as a workload on Google Kubernetes Engine (GKE)?<br><br>

<ol type="A">
<li>Upload the image to Cloud Storage and create a GKE service
        referencing the image.</li>
<li>Upload the image to Cloud Storage and create a GKE deployment
        referencing the image.</li>
<li>Upload the image to Artifact Registry and create GKE deployment
        referencing the image.</li>
<li>Upload the image to Container Registry and create a Kubernetes
        Service referencing the image.</li>
</ol>  

<br>

<ins>Correct Answer: C</ins>

In order to deploy a Docke image of your application on GKE you need to
upload the image to Artifact Registry and create GKE deployment
referencing the image.

Here are some useful links:

- Artifact Registry overview:
  <https://cloud.google.com/artifact-registry/docs/overview>
- Overview of deploying workloads:
  <https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview>

##

19. Which programming languages are supported by Google Cloud Functions?<br><br>

<ol type="A">
<li>Java.</li>
<li>Python.</li>
<li>Ruby.</li>
<li>All of the above.</li>
</ol>

<br>

<ins>Correct Answer: D</ins>

Google Cloud Functions supports the following programming languages:

- Java
- Python
- Ruby
- Node.js
- Go

You can write your functions in any of these languages and deploy them to Cloud Functions.

Here are some useful links:
- Google Cloud Functions documentation:
<https://cloud.google.com/functions>

##

20. Which of the following statements is true about Google Cloud
    Functions?<br><br>

<ol type="A">
<li>It allows developers to write and deploy code without worrying
        about server infrastructure</li>
<li>It is only compatible with Google Cloud Platform services</li>
<li>It requires developers to manage their servers and
        infrastructure</li>
<li>It is a platform for managing cloud storage and data processing</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

Google Cloud Functions is a serverless computing platform that allows
developers to write and deploy code without worrying about server
infrastructure. Cloud Functions will automatically manage the servers
and infrastructure needed to run your code, so you can focus on writing
code.

Cloud Functions is compatible with a variety of Google Cloud Platform
services, including Cloud Storage, Cloud Pub/Sub, and Cloud Firestore.
However, it is not limited to Google Cloud Platform services. You can
also use Cloud Functions to interact with third-party services.

Here are some useful links:
- Google Cloud Functions documentation:
<https://cloud.google.com/functions>

##

21. What **database management systems (DBMs)** can be hosted on Google
    Cloud SQL?<br><br>

<ol type="A">
<li>Only MySQL.</li>
<li>Only PostgreSQL.</li>
<li>Only Microsoft SQL Server.</li>
<li>MySQL, PostgreSQL and Microsoft SQL Server.</li>
</ol>

<br>

<ins>Correct Answer: D</ins>

Google Cloud SQL is a fully managed database service that supports
MySQL, PostgreSQL, and Microsoft SQL Server. It allows you to set up,
maintain, manage, and administer your relational databases in the cloud.

Google Cloud SQL provides the following benefits:

- Fully managed: Google Cloud SQL handles all the database
  administration tasks, such as provisioning, patching, backups, and
  replication.
- Secure: Google Cloud SQL provides a secure environment for your
  databases. It includes features such as encryption, access control,
  and auditing.
- Scalable: Google Cloud SQL can scale to meet your needs, from small to
  large enterprise databases.
- Cost-effective: Google Cloud SQL is a cost-effective way to run your
  databases. It offers a variety of pricing options to fit your budget.

Here are some useful links:

- Google Cloud SQL documentation:
  <https://cloud.google.com/sql/docs/>
- Supported database engines:
  <https://cloud.google.com/sql/docs/db-versions>

##

22. What is the main benefit of using Google Cloud Shared VPC?<br><br>

<ol type="A">
<li>It allows you to share virtual machines between multiple
        projects.</li>
<li>It allows you to share billing information between multiple
        projects.</li>
<li>It allows you to share VPC networks and subnets between multiple
        projects.</li>
<li>It allows you to share IAM roles and permissions between
        multiple projects.</li>
</ol>

<br>

<ins>Correct Answer: C</ins>

Shared VPC enables multiple Google Cloud projects to share a common
network configuration, including VPC networks and subnets, which can
help streamline network management and improve security.

Here are some useful links:
- Shared VPC documentation:
  <https://cloud.google.com/vpc/docs/shared-vpc>

##

23. What is the main difference between Google Cloud Internal Load
    Balancer and Google Cloud HTTPS Load Balancer?<br><br>

<ol type="A">
<li>Google Cloud Internal Load Balancer is used for internal traffic
        within a VPC, while Google Cloud HTTPS Load Balancer is used for
        external traffic over the internet.</li>
<li>Google Cloud Internal Load Balancer supports only HTTP traffic,
        while Google Cloud HTTPS Load Balancer supports both HTTP and
        HTTPS traffic.</li>
<li>Google Cloud Internal Load Balancer is a software-based load
        balancer, while Google Cloud HTTPS Load Balancer is a
        hardware-based load balancer.</li>
<li>Google Cloud Internal Load Balancer is a Layer 4 load balancer,
        while Google Cloud HTTPS Load Balancer is a Layer 7 load
        balancer.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

Google Cloud Internal Load Balancer is used for internal traffic within
a VPC, while Google Cloud HTTPS Load Balancer is used for external
traffic over the internet.

Internal Load Balancer forwards traffic between Compute Engine
instances, Kubernetes Engine clusters, and Cloud Run services within a
VPC. HTTPS Load Balancer forwards traffic from external clients to
Compute Engine instances, Kubernetes Engine clusters, and Cloud Run
services within a VPC.

Here are some useful links:

- Internal Load Balancer:
  <https://cloud.google.com/load-balancing/docs/internal>
- HTTPS Load Balancer:
  <https://cloud.google.com/load-balancing/docs/https>

##

24. What is the main difference between Jobs and Services in Google
    Cloud Run?<br><br>

<ol type="A">
<li>Jobs are used for short-lived tasks, while Services are used for
        long-running applications</li>
<li>Jobs are used for batch processing, while Services are used for
        real-time applications.</li>
<li>Jobs are used for background tasks, while Services are used for
        front-end tasks.</li>
<li>Jobs and Services are the same things in Google Cloud Run.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

The main difference between Jobs and Services in Google Cloud Run is
that Jobs are designed for short-lived, batch-style tasks, while
Services are used for long-running, stateless or stateful web
applications.

Here are some useful links:

- Cloud Run services:
  <https://cloud.google.com/run/docs/resource-model#services>
- Cloud Run jobs:
  <https://cloud.google.com/run/docs/resource-model#jobs>

##

25. You have been tasked with the lifecycle configuration of the Google
    Cloud Storage bucket. The lifecycle rule should change the object’s
    class from Standard to Coldline. Choose the correct rule in JSON
    format:<br><br>

<ol type="A">
<li>

```
{
  "rule": [
    {
      "action": {
        "storageClass": "COLDLINE",
        "type": "SetStorageClass"
      },
      "condition": {
        "age": 30
      }
    }
  ]
}
```
</li>
<li>

```
{
  "rule": [
    {
      "action": {
        "storageClass": "NEARLINE",
        "type": "SetStorageClass"
      },
      "condition": {
        "age": 60
      }
    }
  ]
}
```
</li>
<li>

```
{
  "rulesToSet": [
    {
      {
        "storageClass": "COLDLINE",
        "type": "SetStorageClass"
      },
      "condition": {
        "age": 30
      }
    }
  ]
}
```
</li>
<li>

```
{
  "rule": [
    {
      "execute": {
        "SetStorageClass": "COLDLINE",
        "type": "StorageClass"
      },
      "condition": {
        "age": 30
      }
    }
  ]
}
```
</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

Correct lifecycle rule for Google Cloud Storage bucket actions specify
exactly one of the following actions:

- <code>Delete</code>
- <code>SetStorageClass</code>
- <code>AbortIncompleteMultipartUpload</code>

We can immediately exclude answer B as in this rule, we have the
following statement <code>storageClass": "NEARLINE"</code>. Answer C can be excluded
as instead of the rule, the code has a <code>rulesToSet</code> statement, which can’t
be used in the lifecycle rule. The last answer we need to exclude is
answer D. Instead of an <code>action</code> statement, it has an <code>execute</code> statement,
which is incorrect.

Here are some useful links:

- Object Lifecycle Management:
  <https://cloud.google.com/storage/docs/lifecycle>
- Configuration examples for Object Lifecycle Management:
  <https://cloud.google.com/storage/docs/lifecycle-configurations#command-line>

##

26. You have been tasked to upload many files from the on-premises file
    server into the Google Cloud Storage bucket. You want to leverage a
    parallel multi-threaded copy mechanism. Choose the correct
    **gsutil** command:<br><br>

<ol type="A">
<li><code>gsutil cp -r -M dir gs://my-bucket</code></li>
<li><code>gcloud -m cp -r dir gs://my-bucket</code></li>
<li><code>gsutil cp -r dir gs://my-bucket</code></li>
<li><code>gsutil -m cp -r dir gs://my-bucket</code></li>
</ol>

<br>

<ins>Correct Answer: D</ins>

The correct gsutil command to upload many files from the on-premises
file server into the Google Cloud Storage bucket using a parallel
multi-threaded copy mechanism is <code>gsutil -m cp -r dir gs://my-bucket</code>.

The <code>-m</code> flag enables the parallel multi-threaded copy mechanism. The cp
command copies files from the local file system to the cloud, within the
cloud, and between cloud storage providers. The <code>-r</code> flag copies the
entire directory tree, including all subdirectories and files. The <code>dir</code>
is the local directory containing the files to be uploaded.

Here are some useful links:

- gsutil cp command documentation:
  <https://cloud.google.com/storage/docs/gsutil/commands/cp>

##

27. You are planning the migration of 200 Virtual Machines running on
    VMware vSphere from on-premises with a total size of 280 GiB of
    data. Your Internet provider agreed to increase the speed of your
    Internet connection to 1Gbps. What is the fastest way to migrate
    virtual machines to Google Cloud?<br><br>

<ol type="A">
<li>Use <code>gsutil</code> command-line utility with option <code>-m</code></li>
<li>Use Migrate to Virtual Machines service to migrate directly into
        Google Compute Engine</li>
<li>Order Transfer Appliance TA300, copy all the virtual machines
        files onto it. Once data is uploaded to the Cloud Storage
        bucket, use the command: <code>gcloud compute images import my-imported-image --source-file gs://your_gcs_bucket/my_server.vmdk</code></li>
<li>Convert VMware virtual machines into the RAW format and upload
        it to the Cloud Storage bucket. Use command: <code>gcloud compute images import my-imported-image --source-file gs://your_gcs_bucket/my_server.raw</code></li>
</ol>

<br>

<ins>Correct Answer: C</ins>

Using a physical transfer appliance like Transfer Appliance allows you
to transfer a large amount of data quickly, especially when dealing with
a significant volume of data like 280 GiB. It can be more efficient than
relying solely on an internet connection.

Here are some useful links:

- Google Cloud Transfer Appliance:
  <https://cloud.google.com/transfer-appliance/docs/4.0/overview>

##

28. An application owner has informed you that app performance is
    degraded. After checking application performance metrics in Cloud
    Monitoring, the bottleneck has been identified – the PostgreSQL
    database. Cloud Monitoring points to insufficient CPU capacity and
    slow read performance from the database. What steps can be taken to
    improve the performance of the PostgreSQL database? (Select four
    correct answers):<br><br>

<ol type="A">
<li>Increase the CPU capacity of the database instance.
</li>
<li> Add more memory to the database instance.</li>
<li>Optimize the database schema and indexes.</li>
<li>Use a different database management system.</li>
<li>Create read replicas to offload read queries from the primary
        instance.</li>
</ol>

<br>

<ins>Correct Answer: A, B, C and E</ins>

All answers A, B, C and E are valid options. Options A and B increase
the database's performance by adding more CPU capacity and memory. Read
replicas allow the offload of read queries from the primary database
instance and reduce the storage load.

**Database schema** optimisation involves designing the database
structure (tables, relationships, data types) for efficiency and data
integrity. It aims to balance normalisation and performance, ensuring
that the schema supports efficient data retrieval and manipulation.

**Index optimisation** is the process of strategically creating indexes
on frequently used columns in the database. Indexes improve query
performance by enabling rapid data lookup. However, it's essential to
strike a balance between the number and size of indexes to avoid
overloading the database with unnecessary indexing.

Answer D doesn’t solve the problem we are facing.

Here are some useful links:

- Google Cloud SQL Operational guidelines:
  <https://cloud.google.com/sql/docs/postgres/operational-guidelines>
- Edit Cloud SQL Instance:
  <https://cloud.google.com/sql/docs/postgres/edit-instance>
- Monitor Cloud SQL instances:
  <https://cloud.google.com/sql/docs/postgres/monitor-instance>

##

29. As an operations team member, you have been tasked to create a
    notification channel in Google Cloud operations suite. What are the
    valid options for delivering notifications?<br><br>

<ol type="A">
<li>Email, mobile app, SMS, Pub/Sub.</li>
<li>Email, mobile app, Pub/Sub, Webhooks.</li>
<li>Email, PagerDuty, SMS.</li>
<li>Email, mobile app, PagerDuty, SMS, Slack, Webhooks, Pub/Sub.</li>
</ol>

<br>

<ins>Correct Answer: D</ins>

The valid options for delivering notifications in Google Cloud
Operations Suite include: Email, mobile app, PagerDuty, SMS, Slack,
Webhooks, and Pub/Sub. You can use these channels to receive
notifications and alerts about incidents and issues in your Google Cloud
environment. Each option serves a different purpose and can be
configured based on your specific notification needs.

Here are some useful links:

- Create and manage notification channels:
  <https://cloud.google.com/monitoring/support/notification-options>

##

30. Choose correct identities where IAM roles can be granted.<br><br>

<ol type="A">
<li>Google account and a Service account.</li>
<li>Google group, Cloud Identity domain.</li>
<li>Google account, a service account, Google group, Google
        Workspace domain and a Cloud Identity domain.</li>
<li>Google Workspace domain and a Cloud Identity domain.</li>
</ol>

<br>

<ins>Correct Answer: C</ins>

You can grant IAM roles to these various identities to manage
permissions and access control within the Google Cloud Platform to the
following identities: Google account, a service account, Google group,
Google Workspace domain and a Cloud Identity domain.

Here are some useful links:

- IAM basic and predefined roles reference:
  <https://cloud.google.com/iam/docs/understanding-roles>
- Manage access to projects, folders, and organisations:
  <https://cloud.google.com/iam/docs/granting-changing-revoking-access>

##

31. Which of the following options is a way to provide a group of data
    scientists with access to a 10 GB data set acquired from a
    third-party research firm and minimise the steps they will have to
    take to access it from their statistics programs written in R, while
    also giving each scientist their dedicated VM with the data
    available in the VM's file system?<br><br>

<ol type="A">
<li>Load the dataset into BigQuery.</li>
<li>Use Cloud Storage to store the dataset.</li>
<li> Use a disk with the data to create a source image, then create
        VMs from the source image.</li>
<li>Store the dataset in Google Drive.</li>
</ol>

<br>

<ins>Correct Answer: C</ins>

The best approach is to create a source image from a disk that contains
the dataset, and then use that image to create VM instances for each
data scientist. This ensures that each scientist gets a dedicated VM
with the data preloaded in the VM's file system, minimising the setup
and access steps.

Here are some useful links:

- Create custom images:
  <https://cloud.google.com/compute/docs/images/create-custom>

##

32. Which command can be used to create VPC?<br><br>

<ol type="A">
<li><code>gcloud compute create networks</code></li>
<li><code>gcloud compute networks create</code></li>
<li><code>gsutil networks vpc create</code></li>
<li><code>kubectl compute networks create</code></li>
<li><code>gcloud vpc networks create</code></li>
</ol>

<br>

<ins>Correct Answer: B</ins>

The only valid Answer is B. In the past, we could create a command from
Answer E, but the command has been deprecated and is no longer
recommended for use.

Here are some useful links:
- Create and manage VPC networks:
  <https://cloud.google.com/vpc/docs/create-modify-vpc-networks#gcloud>

##

33. After a successful proof of concept with Google Cloud, you have been
    tasked to create a production Cloud SQL database. As a precaution,
    you would like to enable deletion protection on your production
    Cloud SQL database. Which command can be used to perform this task?<br><br>

<ol type="A">
<li><code>gcloud sql instances create INSTANCE_NAME --deletion-protection</code></li>
<li><code>gcloud compute sql create instances INSTANCE_NAME --deletion-protection</code></li>
<li><code>gsutil compute sql instances create INSTANCE_NAME --no-delete</code></li>
<li><code>gcloud sql instances patch [INSTANCE_NAME] --no-deletion-protection</code></li>
</ol>

<br>

<ins>Correct Answer: A</ins>

To enable deletion protection on a production Cloud SQL database, you
can use the following command: <code>gcloud sql instances patch [INSTANCE_NAME] --deletion-protection</code>. This command will patch the
existing instance with the deletion-protection property set to true.

Here are some useful links:

- Setting deletion protection on a new instance:
  <https://cloud.google.com/sql/docs/mysql/deletion-protection>

##

34. Which roles are necessary to check quotas for a project?<br><br>

<ol type="A">
<li>Project Owner (<code>roles/owner</code>), Project Editor (<code>roles/editor</code>) and
        Quota Viewer (<code>roles/servicemanagement.quotaViewer</code>).</li>
<li>Project Owner (<code>roles/owner</code>).</li>
<li>Quota Viewer (<code>roles/servicemanagement.quotaViewer</code>).</li>
<li>Quota Administrator (<code>roles/servicemanagement.quotaAdmin</code>).</li>
<li>Project Owner (<code>roles/owner</code>) and Quota Administrator
        (<code>roles/servicemanagement.quotaAdmin</code>).</li>
<li>All of the preceding.</li>
</ol>

<br>

<ins>Correct Answer: A</ins>

The Project Owner role has all of the permissions necessary to check
quotas for a project. The Project Editor role also has all of the
permissions necessary to check quotas for a project, except for the
ability to create and delete quotas. The Quota Viewer role has the
permission to view quotas for a project.

Here are some useful links:

- IAM basic and predefined roles reference:
<https://cloud.google.com/iam/docs/understanding-roles>

##

35. What are the options to batch load data into BigQuery?<br><br>

<ol type="A">
<li>Avro.</li>
<li>CSV, JSON.</li>
<li>ORC.</li>
<li>PHP</li>
<li>AVRO, CSV, JSON, ORC.</li>
</ol>

<br>

<ins>Correct Answer: E</ins>

You can load data into BigQuery using various file formats, including
AVRO, CSV, JSON, and ORC, among others. These formats allow you to
import data in bulk for analysis and querying within BigQuery.

Here are some useful links:

- Introduction to loading data:
  <https://cloud.google.com/bigquery/docs/loading-data>

##

36. Which of the following is an appropriate use case for Google
    Dataflow?<br><br>

<ol type="A">
<li>Running a web server and serving HTTP requests.</li>
<li>Generating interactive visualisations of large datasets.</li>
<li>Processing streaming data in real time.</li>
<li>Storing and querying data in a distributed data warehouse.
</li>
</ol>

<br>

<ins>Correct Answer: C</ins>

Google Dataflow is a stream and batch data processing service
well-suited for handling and processing streaming data in real time. It
allows you to build data pipelines that can ingest, transform, and
analyse data as it arrives, making it a powerful tool for real-time data
processing.

Here are some useful links:

- Dataflow overview:
  <https://cloud.google.com/dataflow/docs/overview>

##

37. Choose the correct statement about Google Cloud VPCs and CIDR
    ranges:<br><br>

<ol type="A">
<li>You can create one CIDR range for each VPC.</li>
<li>You can create a CIDR range for each subnet.</li>
<li>You can create a CIDR range for each region.</li>
<li>You can create a CIDR range for each zone.</li>
</ol>

<br>

<ins>Correct Answer: B</ins>

A VPC network can have one or more subnets. Each subnet must have its
own CIDR range. The CIDR range for a subnet must be a subset of the CIDR
range for the VPC network.

Here are some useful links:

- VPC Subnets: <https://cloud.google.com/vpc/docs/subnets>

##

38. You want to implement an infrastructure as a Code approach regarding
    infrastructure deployment in your company. Terraform was brought to
    your attention, and you would like to try it out. Which order of
    terraform commands allows you to deploy your code successfully?<br><br>

<ol type="A">
<li><code>terraform create</code></li>
<li><code>terraform apply, terraform init</code></li>
<li><code>terraform init, terraform plan, terraform apply</code></li>
<li><code>terraform configure, terraform apply, terraform init</code></li>
</ol>

<br>

<ins>Correct Answer: C</ins>

To successfully deploy infrastructure using Terraform, the correct order
of Terraform commands is: <code>terraform init, terraform plan, terraform
apply</code>.

Here's the explanation of each command in the correct sequence:

- <code>terraform init</code>: This command initialises the Terraform environment,
  downloads necessary providers and modules, and sets up the working
  directory for your configuration.
- <code>terraform plan</code>: This command generates an execution plan that
  describes what Terraform will do to achieve the desired state defined
  in your configuration. It allows you to review the changes before
  applying them.
- <code>terraform apply</code>: This command applies the changes defined in your
  Terraform configuration to create or update the infrastructure
  resources as per your plan.

The order of these commands is essential for a successful and controlled
infrastructure deployment using Terraform.

Here are some useful links:

- Basic CLI Features:
  <https://developer.hashicorp.com/terraform/cli/commands>

##

39. Before migration to Google Cloud, your developer’s team used
    RabbitMQ as a message broker. After successfully migrating all
    applications, you would like to use cloud native technologies.
    Choose the correct product that will allow you to use messaging
    services in Google Cloud.<br><br>

<ol type="A">
<li>Dataflow.</li>
<li>Dataproc.</li>
<li>Pub/Sub.</li>
<li>BigQuery.</li>
</ol>

<br>

<ins>Correct Answer: C</ins>

Pub/Sub is a fully managed real-time messaging service that allows you
to send and receive messages between independent applications. It is a
highly scalable and reliable service that can be used to build various
applications, such as real-time chat, social media feeds, and IoT device
monitoring.

Here are some useful links:

- Pub/Sub overview: <https://cloud.google.com/pubsub/docs/overview>

##

40. You are considering using Managed Instance Groups in Compute Engine
    configured with an autoscaling policy. What are valid autoscaling
    policy metrics?<br><br>

<ol type="A">
<li>Average CPU utilisation.</li>
<li>HTTP load balancing serving capacity.</li>
<li>Cloud Monitoring metrics.</li>
<li>All of the above.</li>
</ol>

<br>

<ins>Correct Answer: D</ins>

All of the above are valid autoscaling policy metrics for Managed
Instance Groups in Compute Engine.

To use Cloud Monitoring metrics, you must first create a metric you want
to use for autoscaling. You can then configure your autoscaling policy
to scale based on the metric value.

Here are some examples of Cloud Monitoring metrics that you can use for
autoscaling:

- CPU utilisation.
- Memory usage.
- Disk usage.
- Network traffic.
- Custom metric.

Here are some useful links:

- Autoscaling groups of instances:
  <https://cloud.google.com/compute/docs/autoscaler>

##

41. What are potential use cases for Google Cloud Functions? (Select two
    correct answers):<br><br>

<ol type="A">
<li>Triggering real-time data processing tasks.</li>
<li>Building and deploying web applications.</li>
<li>Automating infrastructure management tasks.</li>
<li>Running long-term, resource-intensive computations.</li>
</ol>

<br>

<ins>Correct Answer: A and C</ins>

Google Cloud Functions is a serverless computing platform that allows
you to build and run event-driven functions without managing servers or
infrastructure. This makes it ideal for triggering real-time data
processing tasks and automating infrastructure management tasks.

For example, you could use Google Cloud Functions to:

- Process data from a real-time stream, such as a sensor or social media
  feed.
- Automatically scale your infrastructure based on demand.
- Send notifications when certain events occur, such as when a new user
  signs up for your service or when a new file is uploaded to your
  storage bucket.

Google Cloud Functions is a cost-effective and scalable way to run
event-driven functions. It is also easy to use and manage, making it a
good choice for developers of all skill levels.

Here are some useful links:

- Cloud Functions overview:
  <https://cloud.google.com/functions/docs/concepts/overview>

##

42. Which of the following are features of Google Cloud Spanner? (Select
    two correct answers):<br><br>

<ol type="A">
<li>It is a NoSQL database that allows for flexible schema designs.</li>
<li>It is a fully managed relational database service.</li>
<li>It provides strong consistency and HA across multiple regions.</li>
<li>It is designed for low-latency, high-throughput workloads.</li>
</ol>

<br>

<ins>Correct Answer: B, C and D</ins>

Spanner is a good choice for applications that require strong
consistency, high availability, and low latency. It is also a good
choice for applications that need to scale to handle large amounts of
data and traffic.

Here are some useful links:

- Cloud Spanner overview: <https://cloud.google.com/spanner>

<br>

> **_Note:_** The book version of Question 42 incorrectly states that the correct answers are B and C, instead of B, C and D.

##

43. You have been asked to create a firewall rule to allow TCP traffic
    destined to VM1 with IP <code>192.168.1.2</code> on port <code>80</code>. Choose the correct
    command to perform this task.<br><br>

<ol type="A">
<li>

```
gcloud compute firewall-rules create firewall-rule-1 --network NETWORK_NAME --action deny --direction egress --rules tcp --destination-ranges 192.168.1.2/32 --priority 1000
```
</li>
<li>

```
gcloud compute firewall-rules create firewall-rule-1 --network NETWORK_NAME --action allow --direction egress --rules tcp:80 --destination-ranges 192.168.1.2/32 --priority 60
```
</li>
<li>

```
gcloud compute firewall-rules create firewall-rule-1 --network NETWORK_NAME --action allow --direction egress --rules tcp:443 --destination-ranges 192.168.1.2/32 --priority 70 --target-tags webserver
```
</li>
<li>

```
gcloud compute firewall-rules firewall-rule-1 --network NETWORK_NAME --action allow --direction ingress --rules tcp:22 --source-tags database --priority 80 --target-tags webserver
```
</li>
<li>

```
gcloud compute firewall-rules firewall-rule-1 --network NETWORK_NAME --action deny --direction egress --rules tcp --destination-ranges 192.168.1.2/32 --priority 1000
```
<code></code></li>
</ol>

<br>

<ins>Correct Answer: B</ins>

In order to create a firewall rule with the provided requirements, the
command gcloud compute firewall-rules create needs to have the following
parameters:

- <code>--action allow</code>: Allows traffic.
- <code>--direction ingress</code>: Specifies that the rule applies to incoming traffic.
- <code>--rules tcp:80</code>: Permits TCP traffic on port 80.
- <code>--destination-ranges 192.168.1.2/32</code>: Specifies the destination IP address.
- <code>--priority 60</code>: Sets the priority for the rule.

Here are some useful links:

- VPC firewall rules:
  <https://cloud.google.com/firewall/docs/firewalls#create>

##

44. Choose the correct statement about Google Cloud Dataproc. (Select
    two correct answers):<br><br>

<ol type="A">
<li>Dataproc is managed by Apache Spark and RabbitMQ service.</li>
<li>Dataproc supports Windows Server and Ubuntu images.</li>
<li>Dataproc allows you to run it on Google Compute Engine or
        Kubernetes Engine.</li>
<li>Dataproc on GKE doesn’t have separate master and worker nodes.</li>
<li>Dataproc is billed on a per-minute base.</li>
</ol>

<br>

<ins>Correct Answer: C and D</ins>

Dataproc is a managed Spark and Hadoop service that lets you take
advantage of open source data tools for batch processing, querying,
streaming, and machine learning. Dataproc automation helps you create
clusters quickly, manage them easily, and save money by turning clusters
off when you don't need them.

Here are some useful links:

- Dataproc overview:
  <https://cloud.google.com/dataproc/docs/concepts/overview>

##

45. You would like to analyse logs stored in Cloud Logging in external
    systems. What are the valid external sink destinations?<br><br>

<ol type="A">
<li>Cloud Logging bucket.</li>
<li>BigQuery data set.</li>
<li>Cloud Pub/Sub topic.</li>
<li>Splunk.</li>
<li>All of the above.</li>
</ol>

<br>

<ins>Correct Answer: E</ins>

You can use Cloud Logging sinks to export your logs to a variety of
external destinations, including Cloud Storage, BigQuery, Cloud Pub/Sub,
and Splunk. This allows you to analyze your logs in external systems and
to build custom log processing solutions.

Here are some useful links:

- Routing and storage overview:
  <https://cloud.google.com/logging/docs/routing/overview>

##

46. What are the three types of roles in Google Cloud IAM? (Select three
    correct answers):<br><br>

<ol type="A">
<li>Basic roles.</li>
<li>Predefined roles.</li>
<li>Admin roles.</li>
<li>Custom roles.</li>
</ol>

<br>

<ins>Correct Answer: A, B and D</ins>

Here are some useful links:

- IAM Roles and permissions:
  <https://cloud.google.com/iam/docs/roles-overview>

<br>

> **_Note:_** The book version of Question 46 incorrectly states option B as — _Special roles_, it should instead be — _Predefined roles_.

##

47. What is true about VPC created in auto mode? (Select two correct
    answers):<br><br>

<ol type="A">
<li>When an auto-mode VPC network is created, one subnet from each
        region is automatically created within it.</li>
<li>Those automatically created subnets use a set of predefined IPv4
        ranges that fit within the <code>10.128.0.0/9</code> CIDR block.</li>
<li> When new Google Cloud regions become available, you have to
        create new subnets in those regions manually.</li>
<li>You cannot add more subnets manually to VPC networks in auto
        mode.</li>
</ol>

<br>

<ins>Correct Answer: A and B</ins>

When you create an auto-mode VPC network, Google Cloud automatically
creates one subnet in each region. These subnets use a set of predefined
IPv4 ranges from the <code>10.128.0.0/9</code> CIDR block. As new regions become
available, Google Cloud automatically creates new subnets.

You can also add more subnets manually to auto-mode VPC networks.
However, you must use IP ranges outside the <code>10.128.0.0/9</code> CIDR block.

Here are some useful links:

- Considerations for auto mode VPC networks:
  <https://cloud.google.com/vpc/docs/vpc#auto-mode-considerations>

##

48. Which of the following statements about the type of applications
    deployed on Kubernetes are true?<br><br>

<ol type="A">
<li>A ReplicaSet ensures that a specified number of pod replicas are
        running at any given time.</li>
<li>A Deployment provides declarative updates for pod replicas and
        allows for rollbacks if necessary.
</li>
<li>A StatefulSet is used to manage stateful applications that
        require stable network identities and ordered deployment and
        scaling.</li>
<li>A DaemonSet ensures that a pod runs on every node in a cluster.</li>
<li>All of the above</li>
</ol>  

<br>

<ins>Correct Answer: E</ins>

All of the above statements about the type of applications deployed on
Kubernetes are true.

- A ReplicaSet ensures that a specified number of pod replicas are
  running at any given time. This is useful for running stateless
  applications, such as web servers, that can be scaled up or down
  horizontally.
- A Deployment provides declarative updates for pod replicas and allows
  for rollbacks if necessary. This makes it easier to manage and update
  applications over time.
- A StatefulSet is used to manage stateful applications that require
  stable network identities and ordered deployment and scaling. This is
  useful for running applications such as databases, caches, and message
  brokers.
- A DaemonSet ensures that a pod runs on every node in a cluster. This
  is useful for running applications that need to run on every node,
  such as logging agents and monitoring agents.

Here are some useful links:

- ReplicaSets:
  <https://kubernetes.io/docs/concepts/workloads/controllers/replicaset/>
- Deployments:
  <https://kubernetes.io/docs/concepts/workloads/controllers/deployment/>
- StatefulSets:
  <https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/>
- DaemonSets:
  <https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/>

##

49. What types of service accounts are available in Google Cloud IAM?
    (Select more than two correct answers):<br><br>

<ol type="A">
<li>User-managed service accounts.</li>
<li>Default service accounts.</li>
<li>Google-managed service accounts.</li>
<li>Service-specific service agents.</li>
<li>None of the preceding.</li>
</ol>

<br>

<ins>Correct Answer: A, B, C and D</ins>

**User-managed service accounts** are service accounts that you create
and manage. You can use these service accounts to grant access to your
Google Cloud resources for applications and workloads.

**Default service accounts** are service accounts that are automatically
created when you enable certain Google Cloud services. These service
accounts are used by the services to access your Google Cloud resources
on your behalf.

**Google-managed service accounts** are service accounts that are
created and managed by Google. These service accounts are used by Google
Cloud services to access your Google Cloud resources on your behalf.

**Service-specific service agents** are a type of Google-managed service
account that is used by a specific Google Cloud service.
Service-specific service agents are created automatically when you
enable the service.

Here are some useful links:

- Types of service accounts:
  <https://cloud.google.com/iam/docs/service-account-overview#types>
- Google-managed service accounts:
  <https://cloud.google.com/iam/docs/service-account-types#google-managed>

##

50. What statements about Kubernetes Services are true regarding
    exposing a containerised application outside a GKE cluster? (Select
    two correct answers):<br><br>

<ol type="A">
<li>A Service can expose a containerised application to the internet
        using a static IP address and a LoadBalancer type.</li>
<li>A Service can only expose a containerised application to other
        applications running inside the GKE cluster.</li>
<li>A Service can expose a containerised application to the internet
        using an Ingress resource.</li>
<li>A Service cannot expose a containerised application outside a
        GKE cluster.</li>
</ol>

<br>

<ins>Correct Answer: A and C</ins>

Kubernetes Services are a way to expose applications running inside a
Kubernetes cluster to the outside world. Services can be exposed using a
variety of types, including **LoadBalancer**, **NodePort**, and
**ClusterIP**.

**LoadBalancer** type Services expose applications to the internet using
a static IP address. This type of Service is typically used to expose
applications to the public.

**Ingress** type Services expose applications to the internet using
rules that define how traffic is routed to the Service. Ingress
resources are typically used to expose applications to the public more
sophisticatedly, such as by routing traffic to different versions of an
application or terminating TLS traffic.

**NodePort** type Services expose applications to other applications
running inside the Kubernetes cluster by exposing them on a specific
port on each node in the cluster.

**ClusterIP** type Services expose applications to other applications
running inside the Kubernetes cluster by assigning them a unique IP
address within the cluster.

Kubernetes Services are a powerful way to expose applications running
inside a Kubernetes cluster to the outside world. They can be used to
expose applications to the internet, to other applications running
inside the cluster, or to both.

Here are some useful links:

- Kubernetes service:
<https://kubernetes.io/docs/concepts/services-networking/service/>

##