# <p align="right">**Mock Test 1 – Answers**</p>

1.  You want to use Google Cloud free credits to explore Google Cloud’s
    services and prepare for your ACE exam. You plan to stay within the
    limits of the free tier whenever possible so that you won’t run out
    of credits too soon. However, you are asked to provide a payment
    method during the free trial signup. Why do you think this happened?<br><br>

<!-- -->

<ol type="A">
<li>It was a mistake. There is no need to provide credit card details
    because you will receive $300 in credits from Google. You need to
    contact the support team.</li>
<li>Google will transfer $300 to your bank account, so you need to
    share your credit card details during the signup process.</li>
<li>Providing payment details is required for the billing account setup,
    regardless of if you plan to use a paid account or free credits.
    This is also how your identity is verified. You will need to monitor
    your spending because you will be charged once you run out of free
    credits.</li>
<li>Providing payment details is required for the billing account setup,
    regardless of if you plan to use a paid account or free credits.
    This is also how your identity is verified. You won’t be charged,
    even if you run out of free credits. You need to explicitly upgrade
    your account to a paid account for Google to be able to charge you.</li>
</ol>

<br>

<ins>Correct answer: D</ins>

The purpose of this question is to motivate new users of Google Cloud to
take advantage of the \$300 Free Trial offer for their hands-on
explorations. While a credit card is required for account setup, no
charges will be applied once the trial ends unless the user explicitly
allows it.<br>
<https://cloud.google.com/free/docs/free-cloud-features##billing_verification><br>

Discover additional information about the Free Trial and Free Tier
features by visiting this link:<br>
<https://cloud.google.com/free/docs/free-cloud-features>.<br>

##

2.  The CFO has just informed you that the company has decided to switch
    banks, and as a result, a new billing account must be configured and
    attached to all existing and new Google Cloud projects. She is
    asking you, the administrator of the resources, if this can be
    achieved without downtime for production workloads and what happens
    to all pending charges. What applies here?<br><br>

<!-- -->

<ol type="A">
<li>Changing a billing account for a project shouldn’t impact running
    services. You can attach a new active billing account to a project
    at any time by going to the <b>My Project</b> page of the <b>Billing</b>
    section. Pending charges will be billed to the former billing
    account, and all new charges will be billed to a new billing
    account.</li>
<li>Changing a billing account for a project shouldn’t impact running
    services. You can attach a new active billing account to a project
    at any time by going to the <b>My Project</b> page of the <b>Billing</b>
    section. Pending and new charges will be billed to a new billing
    account.</li>
<li>Changing a billing account for a project causes downtime to all
    running services. Therefore, you need to schedule a maintenance
    window to switch the billing accounts on the <b>My Project</b> page of
    the <b>Billing</b> section. Pending charges will be billed to the
    former billing account, and all new charges will be billed to a new
    billing account.</li>
<li>Changing a billing account for a project causes downtime to all
    running services. You need to schedule a maintenance window to
    switch the billing accounts on the <b>My Project</b> page of the
    <b>Billing</b> section. Pending and new charges will be billed to a new
    billing account.</li>
</ol>

<br>

<ins>Correct answer: A</ins>

Billing account changes, even in small companies, are not that uncommon.
When working with Google Cloud, you may need to update your payment
method occasionally. It is important to note that changes to billing
should not impact your workloads, and any pending changes will continue
to be billed to the old account.

For more information, please refer to the following links:<br>
<https://cloud.google.com/billing/docs/how-to/modify-project##change_the_billing_account_for_a_project><br>
<https://cloud.google.com/billing/docs/how-to/modify-project##charges-after-change-billing><br>

##

3.  Your team is preparing to migrate their on-premises workloads to
    Google Cloud. However, they are worried about the bill and
    anticipate that it might be higher than they initially calculated.
    What can you recommend to them to better control their cloud
    spending?<br><br>

<!-- -->

<ol type="A">
<li>They should monitor their projects’ total and forecasted monthly
    costs in billing account reports to ensure only necessary services
    are generating costs.</li>
<li>They should create a budget for the cloud billing account that
    includes all their services in all their projects and set a fixed
    monthly budget amount and alert thresholds. If their spending
    exceeds one of these thresholds, billing admins will receive an
    email notification. No resources will be stopped. Also, they will
    still be able to create new workloads.</li>
<li>They should create a budget for the cloud billing account that
    includes all their services in all their projects and set a fixed
    monthly budget amount. If their spending exceeds the target amount,
    they won’t be able to create new workloads.</li>
<li>They should set a limit on the company’s credit card so that they
    won’t be charged more than the allowed amount.</li>
</ol>

<br>

<ins>Correct answer: B</ins>

While monitoring the monthly spending forecast could be a viable option
(answer A), it's recommended to use a more scalable and automated
approach (answer B). It's important to note that no resources are
automatically stopped when the budget threshold is reached. The user is
simply notified about it and can take action to limit their Google Cloud
spending as they see fit.

For more information, please refer to the following link:<br>
<https://cloud.google.com/billing/docs/how-to/budgets><br>

##

4.  What mechanism prevents users from creating unlimited resources for
    a specific service type while keeping existing workloads unaffected?<br><br>

<!-- -->

<ol type="A">
<li>Quota</li>
<li>Disabling APIs</li>
<li>Cloud billing budget</li>
<li>Limits on a credit card used by cloud billing</li>
</ol> 

<br>

<ins>Correct answer: A</ins>

Quota (answer A) can be set independently for a selected service and can
help to limit the deployed resources, in most cases, depending on its
value, without affecting the running service. However, if you disable
the API (answer B), any running services that use it may be deleted.
Turning off billing (answer C) or having credit card issues (answer D)
may stop your workloads.

##

5.  After installing some patches for the operating system in a Compute
    Engine VM, you noticed the application running on the VM stopped
    working. After lengthy troubleshooting, you decide to rebuild the VM
    and reinstall the application on a clean operating system. The
    problem is that the new VM was assigned a different private IP, and
    users cannot access the application. How can you fix this issue?<br><br>

<!-- -->

<ol type="A">
<li> You must reserve the initial internal IP as the static IP address in
    this VPC. Then, you shut down the VM, edit the network interface,
    select the reserved address, and start the VM.</li>
<li>Private IP addresses are automatically assigned. You can’t assign a
    private IP manually by selecting the one you need. Instead, users
    need to change the IP that they are using to a new one. You must
    send an email to all users that share a new IP address.</li>
<li>You must reserve the initial internal IP as the static IP address in
    this VPC. Then, you must recreate the VM one more time, this time
    selecting the reserved address for a network interface.</li>
<li>You must shut down the VM, edit the network interface, change the IP
    to the initial one, and start the VM.</li>
</ol> 

<br>

<ins>Correct answer: C</ins>

It is not possible to assign a new static internal IP address to a VM
instance that is currently running or has been stopped. Therefore,
options A and D are incorrect. Option B is also incorrect as private
addresses can be manually assigned. To assign a reserved static IP
address to a new VM, as explained in option C, a new VM will need to be
created.

For more information, please refer to the following links:<br>
<https://cloud.google.com/compute/docs/ip-addresses/reserve-static-internal-ip-address##restrictions><br>
<https://cloud.google.com/compute/docs/ip-addresses/reserve-static-internal-ip-address##how_to_reserve_a_static_internal_ip_address><br>

##

6.  You have to run a batch job and have a limited budget for this task.
    To save costs, you are considering creating a managed instance group
    with VMs in a spot provisioning model. But first, you need to verify
    that your script handles the preemption correctly. How can you
    achieve this?<br><br>

<!-- -->

<ol type="A">
<li>You can use spot VMs in a managed instance group and use <code>gcloud compute instances simulate-maintenance-event</code> on VMs to test the
    unexpected termination</li>
<li>You can’t use spot VMs in a managed instance group</li>
<li>You can use spot VMs in a managed instance group, but no mechanism
    is available to help simulate the unexpected termination</li>
<li>You can only use preemptive VMs in a managed instance group, but no
    mechanism is available to help simulate the unexpected termination</li>
</ol>  

<br>

<ins>Correct answer: A</ins>

You can use spot and preemptive instances in a Managed Instance group,
so the answers B and D are incorrect. Note that spot instances are a new
version of preemptive instances, offering more features. There are many
ways to test unexpected termination, and that eliminates the answer C.
One of the possible ways to test spot instances in a Managed Instance
group cloud is the option described in answer A.

Please see the links below for more information:<br>
<https://cloud.google.com/compute/docs/instances/spot##spot-with-instance-groups><br>
<https://cloud.google.com/compute/docs/instances/preemptible><br>
<https://cloud.google.com/compute/docs/instances/simulating-host-maintenance><br>

##

7.  You want to run a daily backup to prevent Compute Engine VM data
    from being accidentally deleted. Which option should you choose?<br><br>

<!-- -->

<ol type="A">
<li>Scheduling <code>gcloud compute images create</code> to run daily so that a new
    VM image will be created every day.</li>
<li>Scheduling <code>gcloud compute instance-templates create</code> to run daily so
    that a new VM instance template will be created every day</li>
<li>Use the Google Cloud console to create a VM similar to an existing
    one via the <b>CREATE SIMILAR</b> option in the <b>VM instances</b> view</li>
<li>Create a daily snapshot schedule for the disks attached to the VM</li>
</ol> 

<br>

<ins>Correct answer: D</ins>

Although every option creates some copy of an existing VM instance,
answer C is a manual approach, and A and B create additional full clones
of the original VM, using more space than daily incremental snapshots
described in answer D, which are also a recommended way for VM instance
backups.

Please see the links below for more information:<br>
<https://cloud.google.com/compute/docs/disks/scheduled-snapshots><br>

##

8.  Your organization has two teams: team 1 creates the frontends, while
    team 2 creates backends for applications. The teams often share
    projects and always use the same billing account. How can the
    finance department calculate the organization’s spending on frontend
    and backend resources separately?<br><br>

<!-- -->

<ol type="A">
<li>By using filters in the <b>Cost breakdown</b> section of the
    <b>Billing</b> view. Each team can select the services they use each
    month and share the report with the finance department.</li>
<li>By using folders. Each team should keep their workloads in a
    dedicated folder in every project. The finance department can verify
    spending by filtering the cost per folder in the <b>Cost breakdown</b>
    section of the <b>Billing</b> view.</li>
<li>By using labels. The teams should tag their resources as <code>team:team-1</code>
    or <code>team:team-2</code>. Billing data should be exported to BigQuery for
    analysis. Queries that return the overall spending for both teams
    can be exported to Looker Studio and shared with the finance
    department.</li>
<li>By using tags. The teams should tag their resources as <code>team-1</code> or
    <code>team-2</code>. Billing data should be exported to BigQuery for analysis.
    Queries that return the overall spending tagged as <code>team-1</code> and <code>team-2</code>
    can be exported to Looker Studio and shared with the finance
    department.</li>
</ol>

<br>

<ins>Correct answer: C</ins>

Manually using filters in the Billing view can lead to user errors and
make it difficult for teams to differentiate their workloads. Answer A
is incorrect. Using folders is not a viable solution because teams
collaborate on the same projects, making answer B also incorrect. This
leaves us with two options, answer C and D, and the question of which
one to use: labels or tags. Policies use tags, while labels are used to
distinguish the workloads owned by each team. Therefore, answer C is the
correct choice.

Please see the links below for more information:<br>
<https://cloud.google.com/compute/docs/labeling-resources##labels_and_tags><br>

##

9.  Which storage volume for a Compute Engine instance is protected
    against a failure in a zone and provides the best balance of
    performance and cost?<br><br>

<!-- -->

<ol type="A">
<li>Regional balanced Persistent Disk volume</li>
<li>Zonal balanced Persistent Disk volume</li>
<li>Regional Cloud Storage bucket</li>
<li>Zonal standard Persistent Disk volume</li>
</ol>

<br>

<ins>Correct answer: A</ins>

The balanced disk is the one offering the best performance-to-cost
ratio, and the regional disk type is the one that offers two copies of
data in two regions in one zone. Hence, the regional balanced Persistent
disk is the correct answer.

Please see the links below for more information:<br>
<https://cloud.google.com/compute/docs/disks##disk-types><br>
<https://cloud.google.com/compute/docs/disks##durability><br>

##

10. What are the advantages of using a managed instance group?<br><br>

<!-- -->

<ol type="A">
<li>High availability – it supports multi-zone deployments, scaling
    based on various metrics, built-in mechanisms for automatically
    patching instances, and auto-healing, which creates a new instance
    in case the old one crashes</li>
<li>High availability – it supports multi-zone deployments, built-in
    mechanisms for automatically patching instances, and auto-healing
    that reboots instances in case of a crash</li>
<li>High availability – it supports multi-zone deployments, scaling up
    based on various metrics, built-in mechanisms for automatically
    patching instances, and auto-healing, which reboots instances in
    case of a crash</li>
<li>High availability – it supports multi-zone deployments, scaling down
    based on various metrics, built-in mechanisms for automatically
    patching instances, and auto-healing, which reboots instances in
    case of a crash</li>
</ol>

<br>

<ins>Correct answer: A</ins>

During your exam, you might come across a question with four answer
options that appear similar. Take a moment to carefully analyze them and
identify any differences. For instance, options C and D may look
identical, but one pertains to scaling up while the other pertains to
scaling down. It's important to note that Instance Groups support both
growing and shrinking. Options C, D, and B are incorrect because
auto-healing recreates VMs rather than rebooting them. As a result,
option A is the correct answer.

For more information on the benefits of instance groups, check out the
link provided:<br>
<https://cloud.google.com/compute/docs/instance-groups##benefits><br>

##

11. Which instance group type would you choose to set up automatic
    management for a group of VMs with persistent data?<br><br>

<!-- -->

<ol type="A">
<li>Managed instance group (stateless)</li>
<li>Managed instance group (stateful)</li>
<li>Unmanaged instance group</li>
<li>All of the above</li>
</ol>

<br>

<ins>Correct answer: B</ins>

The correct answer is B because a stateful Managed Instance Group is
necessary for preserving individual state. The elimination of options C
and D is due to the lack of automatic management in unmanaged instance
groups.

For more information on the distinction between stateless and stateful
Managed Instance Groups, please refer to the provided links:<br>
<https://cloud.google.com/compute/docs/instance-groups/stateful-migs##how_stateful_workloads_are_different_from_stateless_workloads><br>
<https://cloud.google.com/compute/docs/instance-groups##unmanaged_instance_groups><br>

##

12. Which compute model should you choose if you want to run a simple
    event-driven serverless service that processes images right after
    they are uploaded to Google Cloud Storage? You also don’t want to
    worry about the execution environment.<br><br>

<!-- -->

<ol type="A">
<li>Cloud Run</li>
<li>Managed instance group</li>
<li>GKE</li>
<li>Cloud Functions</li>
</ol>

<br>

<ins>Correct answer: D</ins>

If you only need to deliver a code, B and C are not the best choices, as
a platform configuration is required. Answers A and D suggest serverless
services, but for Cloud Run, you will need to deliver a container; for
Cloud Functions, you will only need the code. So, option D is the right
choice. It's essential for test-takers to understand the differences
between services, especially serverless options like Cloud Functions and
Cloud Run.

Read more about Cloud Storage and other triggers in Cloud Functions:<br>
<https://cloud.google.com/functions/docs/calling##2nd-gen-triggers><br>

Read more about Cloud Functions vs Cloud Run:<br>
<https://cloud.google.com/blog/products/serverless/cloud-run-vs-cloud-functions-for-serverless><br>

##

13. Which compute model should you choose if you want to run a stateless
    web-based service that scales based on the number of incoming
    requests and uses no resources when there are no requests? Also,
    your developers want to use their custom build for this service.<br><br>

<!-- -->

<ol type="A">
<li>Cloud Functions</li>
<li>Cloud Run</li>
<li>GKE</li>
<li>Kubernetes</li>
</ol>

<br>

<ins>Correct answer: B</ins>

Kubernetes is a container orchestration system, which makes answer D too
generic to be the correct one. GKE requires some minimal resources and
configuration to be available, which eliminates the answer C. Web-based
services and scale-to-zero are the essential features of Cloud Run,
making B the correct answer.

Read more about the scale to zero feature of Cloud Run:<br>
<https://cloud.google.com/run/docs/overview/what-is-cloud-run##scale-to-zero><br>

Read more to find when to use Cloud Run:<br>
<https://cloud.google.com/run/docs/overview/what-is-cloud-run##when_to_use_services><br>

##

14. Which of the following is true about regional GKE clusters?<br><br>

<!-- -->

<ol type="A">
<li>They can’t be deployed in Autopilot mode</li>
<li>They contain multiple replicas of the control plane, running in
    multiple zones in a region and nodes in multiple or a single zone</li>
<li>They can be changed to zonal at any time</li>
<li>They have one replica of the control plane running in a selected
    zone and nodes in multiple zones</li>
</ol>

<br>

<ins>Correct answer: B</ins>

The answer marked as A is not correct as GKE Autopilot clusters are
always regional in nature and cannot be changed to zonal. This makes the
option marked as C also incorrect. The answer marked as D is also
incorrect because regional clusters replicate the control plane across
multiple zones within a region. Therefore, the correct answer is option
B.

For further information on regional GKE clusters, please refer to the
following link.:<br>
<https://cloud.google.com/kubernetes-engine/docs/concepts/regional-clusters><br>

##

15. How can you isolate a GKE cluster so that it can’t be accessed from
    the internet and at the same time allow outbound internet access for
    the nodes?<br><br>

<!-- -->

<ol type="A">
<li>Deploy a public cluster</li>
<li>Deploy a private cluster with <b>Access control plane using its
    external IP address option</b> enabled</li>
<li>Deploy a private cluster and use Cloud NAT for outbound internet
    traffic</li>
<li>Deploy a private cluster with Private Google Access enabled on a VPC</li>
</ol>

<br>

<ins>Correct answer: C</ins>

When considering whether to have a public or private cluster, it's
important to note that a public cluster is not the right choice as it
can be accessed from the internet. Therefore, a private cluster is the
better option since nodes and pods do not have external IP addresses
(with the public endpoint access disabled to prevent the internet access
to the control plane, which was omitted in this question for
simplicity), preventing external access.

External IP addresses would make a private cluster accessible from the
internet, making choice B incorrect. Private Google Access can only be
used to access Google APIs and services and is enabled on the subnet,
not VPC, so the answer D is also incorrect. NAT is a service that
provides internet access to workloads with private IP, making choice C
the correct answer.

For more information on how to provide outbound internet access for
private nodes, please visit the following link:<br>
<https://cloud.google.com/kubernetes-engine/docs/how-to/private-clusters##private-nodes-outbound><br>

To learn more about private vs public GKE clusters, please visit these
links:<br>
<https://cloud.google.com/kubernetes-engine/docs/concepts/private-cluster-concept##architecture_of_private_clusters><br>
<https://cloud.google.com/kubernetes-engine/docs/concepts/types-of-clusters##isolation-choices><br>

##

16. Which sentence about GKE Autopilot is not true?<br><br>

<!-- -->

<ol type="A">
<li>It can be configured with regional or zonal availability</li>
<li>Resources are provisioned based on workloads</li>
<li>You pay for the resources that are consumed by workloads (per pod)</li>
<li>It’s deployed with a hardened configuration</li>
</ol>

<br>

<ins>Correct answer: A</ins>

To answer this question, we must determine the false statement regarding
GKE Autopilot.

To familiarize yourself with the features of GKE Autopilot, please visit
the provided link:<br>
<https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview##benefits><br>

The link: <https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview##create-cluster> explains that GKE Autopilot is regionally accessible, making option A the correct answer.

##

17. How can you configure Cloud Monitoring and Logging for GKE standard
    cluster mode?<br><br>

<!-- -->

<ol type="A">
<li>No configuration is required as Cloud Monitoring and Logging are
    enabled by default during cluster creation</li>
<li>You need to install Ops Agent inside the nodes and enable FW rules
    to allow incoming traffic on ports <code>20201</code> and <code>20202</code></li>
<li>You need to install Ops Agent inside the nodes and modify the
    <code>config.yaml</code> file by adding <code>gke</code> to the list of monitored systems</li>
<li>Cloud Monitoring and Logging for GKE is supported only for GKE
    autopilot cluster mode</li>
</ol>

<br>

<ins>Correct answer: A</ins>

By default, GKE Autopilot comes with logging and monitoring enabled.
With GKE Standard, Cloud Logging and Cloud Monitoring are also enabled
by default upon creating a new cluster (although you can choose to
disable it by unchecking the corresponding box). This makes answer A the
correct option.

For additional details on setting up Cloud Logging and Cloud Monitoring
during GKE Standard cluster creation, please refer to the link provided:<br>
<https://cloud.google.com/stackdriver/docs/solutions/gke/installing##installing><br>

##

18. You are writing an application and you want to focus on code,
    without having to manage infrastructure. That is why you want to use
    Cloud Functions. But you also want to experiment with some code and
    send just a subset of traffic to every new revision. How can you
    achieve this with Cloud Functions?<br><br>

<!-- -->

<ol type="A">
<li>You must use Cloud Run to split traffic between revisions. This
    can’t be achieved with Cloud Functions.</li>
<li>Traffic splitting between various versions of your code is a Cloud
    Functions second- generation feature, so you need to use this
    version.</li>
<li>Cloud Functions (first and second generation) support the
    traffic-splitting mechanism by default. It doesn’t matter which
    version you use.</li>
<li>You can configure an HTTP(S) load balancer to distribute traffic
    between revisions of Cloud Function deployments.</li>
</ol>

<br>

<ins>Correct answer: B</ins>

Traffic splitting is a flagship Cloud Functions 2<sup>nd</sup> gen
feature.

To learn more about it, visit this link:<br>
<https://cloud.google.com/functions/docs/configuring/traffic-splitting><br>

##

19. Which sentence does not describe Cloud Functions?<br><br>

<!-- -->

<ol type="A">
<li>It supports languages such as Python, Java, Go, and Node.js</li>
<li>You can trigger Cloud Function execution with HTTP/S requests,
    Pub/Sub messages, and Cloud Storage changes, such as a new object
    being created or deleted.
</li>
<li>You are billed only for the time your function is executed</li>
<li>It supports network protocols beyond HTTP/S</li>
</ol>

<br>

<ins>Correct answer: D</ins>

We must determine the false statement regarding Cloud Functions to
answer this question. As it does support multiple language runtimes, can
be triggered with HTTP/S requests, Pub/Sub messages and Cloud Storage
events and is billed for the time it is executed, it leaves D as the
incorrect statement, making it the correct answer.

For more information, please refer to the following link:<br>
<https://cloud.google.com/functions/docs/concepts/execution-environment><br>

##

20. Select the sentence that is not true about Cloud Run.<br><br>

<!-- -->

<ol type="A">
<li>It runs code in response to events</li>
<li>It runs containers in a fully managed environment</li>
<li>It allows you to use any language and any library</li>
<li>It scales automatically</li>
</ol>

<br>

<ins>Correct answer: A</ins>

To answer this question, we need to identify the false statement about
Cloud Run.

You can visit: <https://cloud.google.com/run/docs/overview/what-is-cloud-run> to read statements that will provide a better understanding of Cloud
Run's features.

Cloud Run is a managed platform that allows you to run containers built
from an image with code written in any programming language. It also has
automatic scaling capabilities. The incorrect statement is found in
option A, as it pertains to Cloud Functions, not Cloud Run.

##

21. What are the minimum steps required to deploy a Cloud Run service?<br><br>

<!-- -->

<ol type="A">
<li>Build a container with code that listens to HTTP requests on a
    predefined port. Then, create a service endpoint and deploy the
    container by selecting its image and providing a name for a service
    and a region where it should run. Finally, configure Cloud Logging
    for the Cloud Run service.</li>
<li>Build a container with code that listens to HTTP requests on a
    predefined port. Then, create a source repository and upload the
    image before creating a service endpoint. Finally, deploy the
    container by selecting its image from the source repository and
    providing a name for a service.</li>
<li>Build a container with code that listens to HTTP requests on a
    predefined port, then deploy the container by selecting its image
    and providing a name for a service and a region where it should run.</li>
<li>Build a container with code that listens to HTTP requests on a
    predefined port, then deploy the container on a previously created
    GKE cluster in a selected region.</li>
</ol>

<br>

<ins>Correct answer: C</ins>

This is a type of question where the answers may seem very similar and a
little vague, so it's important to pay attention to small differences in
order to choose the right one. Answer A is incorrect because Cloud
Logging is enabled by default. Answer B is also incorrect because the
question is asking about the minimum steps needed, assuming the
repository is already configured. Answer D is incorrect because Cloud
Run is fully managed and doesn't require a GKE cluster. That leaves us
with answer C, which is the closest to the truth. Although there are
additional steps such as authentication, networking, and security, most
of them have default values that can be used for a minimal
configuration.

It is important to understand that in some cases during the exam, there
is no perfect answer. Therefore, we must eliminate incorrect answers and
select the one closest to the correct answer.

To learn more about deploying Cloud Run, please visit the following
link:<br>
<https://cloud.google.com/run/docs/deploying##service><br>

##

22. You are an instructor who delivers Associate Cloud Engineer exam
    preparation courses. Every time a course starts, you must deploy
    labs for your students. To simplify troubleshooting, all deployments
    must be the same. After the course, labs need to be destroyed to
    avoid costs. How can you prepare your labs efficiently?<br><br>

<!-- -->

<ol type="A">
<li>Use Infrastructure as Code. You can use Google Cloud Platform
    Provider in Terraform to provision your projects and create
    resources. Later, you can use <code>terraform destroy</code> to remove the provisioned workloads.</li>
<li>You should prepare a deploy script and use Cloud Client Libraries to
    access the Google Cloud API programmatically to set up your
    projects. Later, by detaching your billing account from projects,
    you can ensure resources will be deleted.</li>
<li>Use Infrastructure as Code. You can use Google Cloud Platform
    Provider in Terraform to provision your projects and create
    resources. Later, you can delete each project manually to ensure no
    services are running.</li>
<li>You should prepare a deploy script and use Cloud Client Libraries to
    access the Google Cloud API programmatically to set up your projects
    and delete them later.</li>
</ol>

<br>

<ins>Correct answer: A</ins>

There are various ways to create and delete workloads, but in terms of
efficiency, using Terraform is the best option. Writing code or
configuring things manually may take longer than using Terraform.
Terraform can be used for both provisioning and deleting resources,
ensuring that all actions are automated and not prone to human errors,
making them repeatable.

To learn more about using Terraform, please visit the following link:<br>
<https://cloud.google.com/docs/terraform><br>

##

23. What is a good use case for running Cloud Run on Anthos instead of
    using a fully managed Cloud Run?<br><br>

<!-- -->

<ol type="A">
<li> Incorporating Kubernetes’ best practices and creating a better
    bridge between the Dev and Ops teams</li>
<li>Running a flexible serverless platform to deploy workloads in hybrid
    and multi-cloud environments</li>
<li>Simplifying the application deployment and management experience for
    Kubernetes</li>
<li>Ability to scale down to zero</li>
</ol>

<br>

<ins>Correct answer: B</ins>

Cloud Run on Anthos allows for a consistent user experience when running
workloads in hybrid and multi-cloud environments.<br>

Visit <https://cloud.google.com/anthos/run> for more information.<br>

##

24. Your team is designing a business-critical application that is
    expected to go from a small to a massive scale. Which managed
    relational database would you recommend, knowing they need the
    ability to scale the instance without downtime and require strong
    consistency?<br><br>

<!-- -->

<ol type="A">
<li>Cloud SQL</li>
<li>Cloud BigTable</li>
<li>Cloud Firestore</li>
<li>Cloud Spanner</li>
</ol>

<br>

<ins>Correct answer: D</ins>

Only answers A and D are relational databases, eliminating B and C.
Answer D is correct because Cloud Spanner's flagship feature is its
strong consistency.

Learn more about Cloud Spanner consistency at:<br>
<https://cloud.google.com/spanner/docs/true-time-external-con><br>

##

25. While building a truck tracking application for a global logistics
    company, you look for a scalable, low-latency database to store the
    GPS position of thousands of vehicles at a given timestamp. Which
    database should you choose?<br><br>

<!-- -->

<ol type="A">
<li>Cloud SQL</li>
<li>Cloud BigTable</li>
<li>Cloud Firestore</li>
<li>Cloud Spanner</li>
</ol>

<br>

<ins>Correct answer: B</ins>

When dealing with time-series data in a database, BigTable is likely the
best option.

Learn more about BigTable use cases at the following link:<br>
<https://cloud.google.com/bigtable/docs/overview##what-its-good-for><br>

##

26. You are designing a serverless system to analyze real-time data
    streamed by people counting appliances in stores so that your
    analytics team can better understand consumers’ behavior. What would
    be the most critical components of such a system?<br><br>

<!-- -->

<ol type="A">
<li>Real-time data should be streamed to Pub/Sub first so that no event
    is lost in the case of processing bottlenecks. Then, data should be
    parsed through Dataflow and sent to BigQuery, where it will be
    available for the analytics team.</li>
<li>Real-time data should be streamed directly to BigQuery, where it
    will be available for the analytics team.</li>
<li>Real-time data should be streamed to Pub/Sub first so that no event
    is lost in the case of processing bottlenecks. Then, data should be
    parsed through Dataproc and sent to BigQuery, where it will be
    available for the analytics team.</li>
<li>Real-time data should be streamed to Pub/Sub first so that no event
    is lost in the case of processing bottlenecks. Then, data should be
    parsed through Dataproc and sent to BigTable, where it will be
    available for the analytics team.</li>
</ol>

<br>

<ins>Correct answer: A</ins>

To avoid bottlenecks, it is advisable to utilize Pub/Sub. While deciding
between Dataflow and Dataproc can be difficult, the requirement for a
serverless system for stream data processing suggests that Dataflow
should be used.

To gain knowledge of how Pub/Sub integrates with Dataflow and streams to
BigQuery, kindly refer to the given links below:<br>
<https://cloud.google.com/dataflow/docs/concepts/streaming-with-cloud-pubsub><br>
<https://cloud.google.com/pubsub/docs/stream-messages-dataflow><br>
<https://cloud.google.com/dataflow/docs/tutorials/dataflow-stream-to-bigquery><br>
<https://cloud.google.com/dataflow><br>

##

27. Which CLI command can be used to create a Google Cloud Storage
    bucket called ```my-awesome-bucket```?<br><br>

<!-- -->

<ol type="A">
<li>

```cbt mb my-awesome-bucket```</li><li>

```bq mb gs://my-awesome-bucket```</li><li>

```gsutil mb gs://my-awesome-bucket```</li><li>

```gcloud buckets create gs://my-awesome-bucket```</li>
</ol>

<br>

<ins>Correct answer: C</ins>

This query provides a refresher on the various command line tools that
might come up in the exam. The cbt is a tool used in conjunction with
Cloud Bigtable, bq is the command line for BigQuery, gsutil is used for
Google Cloud Storage configuration, and gcloud is used to configure
Google Cloud services. When creating a GCS bucket, both gsutil and
gcloud can be utilized. Option C is the correct response instead of
option D because the proper gcloud command for creating a bucket is
"gcloud storage buckets create", not "gcloud buckets create".

##

28. You are working on an application to help studio photographers share
    session photos with their customers. You have decided to use Google
    Cloud Storage buckets to store photos, but you are worried that
    storing a large number of high-resolution images can be expensive.
    To limit the storage bill, you decided that photos will be available
    for download for 30 days only. How can you achieve this?<br><br>

<!-- -->

<ol type="A">
<li>Use Google Cloud SDK in your application’s code to interact with
    Google Cloud Storage, query the objects’ lifetimes, and delete ones
    that are older than 30 days.</li>
<li>List bucket details in the Google Cloud console in the Google Cloud
    Storage view, order objects by date, and delete the oldest every
    month.</li>
<li>Use the Google Cloud Storage Autoclass feature to automatically
    detect access patterns and move objects to the Archive storage if
    they are not accessed for 30 days.</li>
<li>Use Object Lifecycle with <b>Action</b> set to <code>delete</code> and <b>Condition</b>
    set to <code>age=30</code>.</li>
</ol>

<br>

<ins>Correct answer: D</ins>

While answer A may be correct, it requires coding and time to implement.
Answer B is a manual approach that is susceptible to user errors. Answer
C is incorrect, as Autoclass only changes an object's class and does not
delete it. Answer D is the most convenient and scalable option
available. It involves using Object Lifecycle Management, which
automatically deletes objects that are older than a set age (30 days).

For more information on Object Lifecycle Management, please visit the
following link:<br>
<https://cloud.google.com/storage/docs/lifecycle><br>

##

29. Which of the following storage systems would be the best fit for
    storing users’ home directories?<br><br>

<!-- -->

<ol type="A">
<li>Google Cloud Storage</li>
<li>Persistent Disk</li>
<li>Filestore</li>
<li>Local Disk</li>
</ol>

<br>

<ins>Correct answer: C</ins>

Among the available options, Filestore offers the ability to mount
fileshares on virtual machines in Google Cloud or on-premises clients
for various purposes, including home directories.

##

30. You are designing a standalone application that must survive a
    failure in a Google Cloud region. You decide to create resources in
    two regions, europe-west3 and europe-central2, and build a
    replication mechanism between them. Which network design would be
    the most optimal for this case?<br><br>

<!-- -->

<ol type="A">
<li>One VPC with a subnet in the europe-west3 and europe-central2
    regions</li>
<li>Two VPCs with a subnet in the europe-west3 and europe-central2
    regions</li>
<li>One shared VPC with a subnet in the europe-west3 and europe-central2
    regions</li>
<li>There is no need to create two redundant subnets since the VPC is a
    global, highly available service</li>
</ol>

<br>

<ins>Correct answer: A</ins>

The easiest and most efficient approach would be to create a single VPC
(which is global) with two subnets, one for each region, as proposed in
option A. Option B is also possible, but it would require creating
connectivity between two VPCs via VPC peering or VPN to ensure the
replication of the workloads. Option C suggests using a Shared VPC, but
it may add an extra layer of complexity at this stage since we don't
have enough information about its design. Option D is correct in stating
that VPCs are global, but it's still necessary to connect workloads to
their respective local subnets in each region.

##

31. You used Google Cloud SDK in your code to spin up 500 Compute Engine
    VMs in the same subnet. However, in the Google Cloud console, you
    noticed that only around half of them were successfully deployed.
    What could be the reason for this?<br><br>

<!-- -->

<ol type="A">
<li>Your application ran out of memory</li>
<li>Your subnet was created with a <code>/24</code> mask and you used all of the IP
    addresses</li>
<li>Using Google Cloud SDK is not supported for creating a large number
    of resources</li>
<li>Your Organization Policy only allows you to create 250 VMs per user</li>
</ol>

<br>

<ins>Correct answer: B</ins>

The subnet was likely created with a <code>/24</code> mask, limiting available IP
addresses to around 250, which is insufficient for 500 VMs.

##

32. How can you provide internet access to a Compute Engine VM with only
    a private IP assigned?<br><br>

<!-- -->

<ol type="A">
<li>Internet access will only be available for a VM with a public IP
    assigned</li>
<li>Use Cloud NAT</li>
<li>You need to add a default route of <code>0.0.0.0/0</code> to the internet in the
    VPC where a VM is running</li>
<li>You need to add a DNS entry of <code>8.8.8.8</code> to the VM’s networking
    configuration</li>
</ol>

<br>

<ins>Correct answer: B</ins>

The correct answer is B because Cloud NAT allows virtual machine
instances with private IP addresses to access resources outside their
VPC network, such as the internet. Option A is incorrect because Cloud
NAT enables outbound connections for VMs with private IP addresses.
Option C is not necessary as there is no need to create a default route.
DNS is required for resolving web addresses, but it won't work without
NAT.

For more information about Cloud NAT, visit the following link:<br>
<https://cloud.google.com/nat/docs/overview><br>

##

33. Which load balancer type would best fit a globally accessible
    external non-HTTPS application?<br><br>

<!-- -->

<ol type="A">
<li>External network TCP/UDP load balancer</li>
<li>Global external TCP/SSL Proxy</li>
<li>Global external HTTP(S) load balancer</li>
<li>None of them</li>
</ol>

<br>

<ins>Correct answer: B</ins>

To achieve global accessibility for the load balancer, options B and C
are available. However, option C is not applicable as it only supports
HTTP(S) based applications. On the other hand, option B is the correct
choice as it enables the configuration of other ports for global
external TCP/SSL proxy.

For further guidance on selecting the appropriate load balancer, please
refer to this link:<br>
<https://cloud.google.com/load-balancing/docs/choosing-load-balancer><br>

##

34. You are connecting your on-premises environment with Google Cloud.
    However, your on-premises router doesn’t support BGP for exchanging
    routes. Which option can you choose to connect to Google Cloud?<br><br>

<!-- -->

<ol type="A">
<li>Dedicated Interconnect</li>
<li>Partner Interconnect</li>
<li>HA VPN</li>
<li>Classic VPN</li>
</ol>

<br>

<ins>Correct answer: D</ins>

On-premises VPN devices that don't support BGP can only use Classic VPN
tunnels to configure static routing.

For more information on Classic VPN, visit the following link:<br>
<https://cloud.google.com/network-connectivity/docs/vpn/deprecations/classic-vpn-deprecation##supported-configs><br>

##

35. You are working on an application that will be running inside a
    Compute Engine VM. The application will index files uploaded to a
    Google Cloud Storage bucket, searching for specific text patterns.
    How can the application access the bucket?<br><br>

<!-- -->

<ol type="A">
<li>The service account that is assigned to the VM needs to have Google
    Cloud Storage access permissions such as Storage Admin for
    interacting with the bucket</li>
<li>The VM can access the objects in the same project as the bucket if
    Private Service Access is enabled on a VPC</li>
<li>If a user who creates the VM has the Compute Admin role, the VM will
    be able to access the objects</li>
<li>The default service account that’s assigned to a VM during
    deployment has Google Cloud Storage access permissions by default,
    so the VM can interact with the bucket</li>
</ol>

<br>

<ins>Correct answer: A</ins>

To authenticate an application, one option is to use a service account
(custom or a default one) that is connected to a Compute Engine
instance. This allows any application operating on the instance to
authenticate as the service account. The attached service account can be
granted the IAM Storage Admin role (it doesn’t have it by default),
which permits access to Google Cloud Storage resources.

For additional information about service accounts, visit:<br>
<https://cloud.google.com/iam/docs/service-account-overview##what-are-service-accounts><br>

##

36. Starting next year, your company must comply with regulatory
    requirements to store data in the European Union. How can this be
    achieved?<br><br>

<!-- -->

<ol type="A">
<li>By using the <code>gcloud asset search-all-resources</code> command to search for
    assets outside the EU.</li>
<li>By creating VPC subnets only in EU regions. Here, resources can only
    be created in regions where a subnet exists.</li>
<li>By using an organization policy to limit the regions where resources
    can be deployed to the EU ones. This will apply to new resources
    only, so an audit needs to be conducted to identify which existing
    resources need to be migrated.</li>
<li>By using an organization policy to limit the regions where resources
    can be deployed to the EU ones. This will apply to existing and new
    resources, so it has to be done during a maintenance window to
    ensure there’s no impact on existing services.</li>
</ol>

<br>

<ins>Correct answer: C</ins>

It is not recommended to use method A as it is a manual approach and not
very efficient. Method B can prevent users from creating resources
outside of the EU, but only those that use VPC. The organization policy
is the preferable option for controlling the deployment location of
resources, but it can only be applied to new workloads. Therefore,
option D is incorrect.

You can find additional information on Restricting Resource Locations by
visiting the link provided below:<br>
<https://cloud.google.com/resource-manager/docs/organization-policy/defining-locations><br>

##

37. You are working as a networking administrator in a global company.
    Your current assignment is to plan networking for all new Google
    Cloud projects to simplify its management overhead. However, you
    want to address the following problem with existing projects: every
    time Google launches a new region, developers contact you and ask
    for a subnet in a new region. As a result, you log in to existing
    projects one by one and manually add a new subnet. How can you
    simplify this process?<br><br>

<!-- -->

<ol type="A">
<li>Use a Shared VPC in the custom mode</li>
<li>Use a Shared VPC in auto mode</li>
<li>Use a VPC in custom mode</li>
<li>Use a VPC in auto mode</li>
</ol>

<br>

<ins>Correct answer: B</ins>

We are asked how to simplify management overhead. Using Shared VPC, a
centrally managed networking, can help us achieve this.

Option A and B are both possible answers, but B is the correct one
because using VPC in auto mode ensures that Google will automatically
add a subnet in any new regions that become available.

For more information on the auto mode VPC network, visit this link:<br>
<https://cloud.google.com/vpc/docs/vpc##subnet-ranges><br>

##

38. Your organization still uses legacy tools that require service
    account keys. You must ensure the keys are used only by the entitled
    tools. Which option will help you to achieve this?<br><br>

<!-- -->

<ol type="A">
<li>Cloud Logging</li>
<li>Service Account Insights</li>
<li>Cloud Monitoring</li>
<li>Cloud Audit Logs</li>
</ol> 

<br>

<ins>Correct answer: D</ins>

There are a couple of options available, such as Cloud Logging and Cloud
Monitoring, but in this particular situation, it's important to consider
that a key can be used with a service account to not only manage Google
Cloud services, but also to access data. For instance, if a GCS object
in a bucket was deleted, Audit Logs would record this event if Data
Read/Write logs in Audit Logs were enabled. This could potentially
provide more information to help track down the issue.

On another note, Google is introducing a new feature called Activity
Analyzer, which can be used to monitor service account key usage.

To learn more about this feature, please visit the following link:<br>
<https://cloud.google.com/policy-intelligence/docs/activity-analyzer-service-account-authentication><br>

##

39. You supervise three teams of developers: team a, team b, and team c.
    Those teams create and use multiple Google Cloud projects for their
    workloads. Following Google’s recommendations, how can you ensure
    you have view access to all of them?<br><br>

<!-- -->
<ol type="A">
<li>Create a root folder for your teams and add individual folders for
    each team under the root folder. Ensure team members only have a
    Project Creator role at their team’s folder level. The Project
    Viewer role needs to be assigned to you at the root folder level.</li>
<li>The Project Viewer role needs to be assigned to you in every project
    individually.</li>
<li>The Project Viewer role needs to be assigned to you at the
    organization level.</li>
<li>Create a root folder for your teams and add individual folders for
    each team under the root folder. Ensure team members only have a
    Project Creator role at their team’s folder level. The Project
    Viewer role needs to be assigned to you at every team’s folder
    level.</li>
</ol> 

<br>

<ins>Correct answer: A</ins>

To grant you access to your team's folders, it is most efficient to
assign you the Project Viewer role at the root folder. This will
automatically distribute access to all underlying folders, as mentioned
in answer A. While answer B is also a potential solution, it requires
manual tracking of newly created projects to provide you access. Answer
C suggests assigning permissions at the organizational level, but this
may include other projects that you should not have access to. Answer D
is similar to answer A, but suggests manually adding your account to
each folder, which requires tracking new projects and remembering to add
access.

##

40. Which is not the recommended best practice for providing access to
    Google Cloud resources?<br><br>

<!-- -->

<ol type="A">
<li>Attach IAM roles to groups instead of individual users</li>
<li>Use the principle of least privilege</li>
<li>Use Basic roles</li>
<li>Use Predefined roles</li>
</ol>

<br>

<ins>Correct answer: C</ins>

Using basic roles in production environments is not advised due to their
broad scope.

For more information on the risks, visit:<br>
<https://cloud.google.com/iam/docs/roles-overview##basic>.<br>

##

41. You deployed an application on a Compute Engine VM, which generates
    unstructured logs that must be stored for 7 years. After a few
    weeks, you notice that the log volume it generates is too high to be
    stored locally on a Persistent Disk. To reduce spending, you decide
    to send logs to an external system. Which option would be the best
    fit?<br><br>

<!-- -->

<ol type="A">
<li>Add functionality to your application’s code to send logs to the
    Google Cloud Storage archive class bucket. Set Object Lifecycle on
    the bucket to delete data after 7 years.</li>
<li>Add functionality in your application’s code to send logs to a
    syslog appliance on-premises, backed by a storage array that can be
    used for archiving.</li>
<li>No code changes are required. Install Ops Agent, which will collect
    and process logs and send them to Cloud Logging without additional
    setup. Create a log sink to send the application logs to a log
    bucket and set its retention to 7 years.</li>
<li>Add functionality to your application’s code using client libraries
    to structure and send logs to the Cloud Logging API. Create a log
    sink to send the application logs to a log bucket and set its
    retention to 7 years.</li>
</ol>

<br>

<ins>Correct answer: D</ins>

The scenario involves a situation where the size of the logs has
surpassed the capacity of the attached Persistent Disk and the
administrator is seeking a cost-effective solution to redesign the
system. While increasing the disk size is an option, the aim is to
minimize expenses, hence the search for an alternative solution. Option
A involves modifying the code and utilizing a log parsing tool. However,
it may result in additional costs due to the increased usage of the
archive class, which charges read operations. Option B requires
on-premises hardware, which may require purchasing and maintenance
costs, depending on the system's architecture. Option C isn't suitable
if the application isn't natively supported by the Ops Agent, as
additional configuration and scripting may be necessary. Option D is the
best fit as it requires minor modifications to the code, but structured
logs will be accessible in Cloud Logging for further analysis and will
be stored for up to 7 years.

##

42. The security team in your organization contacted you, the
    application owner, and asked you to troubleshoot their access to
    Audit Logs for your project. They wanted to examine logs from Google
    Cloud Storage for object upload and deletion on your buckets. But
    when they accessed Cloud Logging, they could only see logs related
    to bucket creation. How can you fix this?<br><br>

<!-- -->

<ol type="A">
<li>The security team needs a Logging Admin role to be able to see Audit
    Logs.</li>
<li>You need to enable Data Access Logs for the Google Cloud Storage
    service. Also, the security team needs to be added to “exempted
    principals” in the Google Cloud Storage data audit log
    configuration.</li>
<li>You need to enable Data Access Logs for the Google Cloud Storage
    service. Also, the security team needs a Private Log Viewer role to
    be able to see Data Access logs.</li>
<li>The security team needs a Private Log Viewer role to be able to see
    Admin Activity logs.</li>
</ol>

<br>

<ins>Correct answer: C</ins>

If you want log the following operations: read, create, or modify an
object on Google Cloud Storage, you need to enable Data Access audit
logs. These operations are not automatically logged in Cloud Logging. To
access Data Access audit logs, you must have the Private Log Viewer
role.

For more information on Data Access Audit Logs, visit:<br>
<https://cloud.google.com/storage/docs/audit-logging##available-logs><br>

For more information on Private Log Viewer rile, visit:<br>
<https://cloud.google.com/iam/docs/audit-logging##audit_log_permissions><br>

##

43. You want to configure a VPC in a newly created project. What is the
    first step you need to do to be able to create a VPC?<br><br>

<!-- -->

<ol type="A">
<li>Enable the Compute Engine API</li>
<li>Go to <b>VPC Networks</b>, select <b>CREATE VPC NETWORK</b>, and start
    configuring the VPC</li>
<li>Enable the Cloud Networking API</li>
<li>You don’t need to do anything – the default VPC is ready to use once
    a new project is created</li>
</ol>

<br>

<ins>Correct answer: A</ins>

When starting a new project using Google Cloud UI (as of writing this
question), it is necessary to enable the Compute Engine API before
creating a VPC. This question serves as a reminder that APIs must be
enabled for a service to be used. Some services may have multiple
dependencies and require the activation of more than one API.

To learn more about Google Cloud API, please follow the link provided:<br>
<https://cloud.google.com/apis/docs/getting-started##enabling_apis><br>

##

44. Your team wishes to consolidate the monitoring of all Compute Engine
    VMs deployed in multiple projects in one place. However, they also
    want to be able to view VM metrics per individual project. How can
    they achieve this most effectively?<br><br>

<!-- -->

<ol type="A">
<li>They should decide which of the existing projects will become a new
    scoping project and add all existing projects to this one.</li>
<li>They should create a new project dedicated to monitoring and add
    other projects to the scoping project.</li>
<li>This can only be achieved by exporting metrics to a third-party
    monitoring tool.</li>
<li>They should decide which of the existing projects will become a new
    scoping project and add all existing projects to this one. They
    should use filters and customized charts to monitor VMs for
    individual projects.</li>
</ol> 

<br>

<ins>Correct answer: B</ins>

It is recommended to set up a separate project specifically for
consolidating monitoring data from other projects. This will allow for
easier management of access to the monitoring data.

For further information on how to configure a metrics scope for multiple
projects, please visit:<br>
<https://cloud.google.com/monitoring/settings/multiple-projects><br>
<https://cloud.google.com/monitoring/settings##create-multi><br>

##

45. How can you create a group that includes both users and service
    accounts?<br><br>

<!-- -->
<ol type="A">
<li>In the Google Cloud console, at the organization level, go to the
    <b>Groups</b> section of IAM, create a group, and add all members and
    their roles.</li>
<li>Log in to the Admin console as a superadmin at
    <a>https://admin.google.com</a>, go to <b>Directory</b> | <b>Group</b>, create a
    new group, and add its members. Next, add the group members.</li>
<li>Log in to the Admin console as a superadmin at
    <a>https://admin.google.com</a>, go to <b>Directory</b> | <b>Group</b>, create a
    new group, and add its members. Next, add the group members.
    Finally, log in to the Google Cloud console and verify that the
    group exists.</li>
<li>You can’t create a group that consists of both users and service
    accounts.</li>
</ol>  

<br>

<ins>Correct answer: A</ins>

Although adding a service account to a group is not the preferred option
(as described in this link:
<https://cloud.google.com/iam/docs/best-practices-service-accounts##groups>),
it is still possible to do so through the Groups view in the IAM
section. It should be noted that the Admin console is not where service
accounts are managed; they can be managed in the Service Accounts view
of the IAM section. A group can have a mix of users and service
accounts.

##

46. A support team should only be able to view monitoring dashboards
    without access to other resources in all projects under the
    <code>production</code> folder. What option would follow Google’s recommendation in this scenario?<br><br>

<!-- -->
<ol type="A">
<li>Create a group for the support team and assign a Project Viewer role
    to the group at the <code>production</code> folder level.</li>
<li>Assign a Project Viewer role to individual users at the <code>production</code>
    folder level.</li>
<li>Create a group for the support team and assign a Project Viewer role
    to the group at the <code>production</code> folder level. In the individual
    projects, assign the Monitoring Viewer role to the group.</li>
<li>Create a group for the support team and assign a Monitoring Viewer
    role to the group at the <code>production</code> folder level.</li>
</ol>  

<br>

<ins>Correct answer: D</ins>

Users can gain Project Viewer access by following the instructions
provided in answer A. This will allow them to view more than just
monitoring dashboards. It is important to note that answer B is
incorrect as it is recommended to add users to a group instead of
assigning roles to individual users. Answer C suggests giving users
higher permissions (Project Viewer) on the folder level, but assigning
lesser permissions on the project level will not make any difference. To
ensure that users have the minimal required permissions to complete
their tasks, it is best to assign appropriate permissions on the folder
level, as demonstrated in answer D.

##

47. You accidentally applied the <code>gcloud projects delete project1</code> command
    instead of <code>gcloud projects delete project2</code>. How can you revert this action?<br><br>

<!-- -->
<ol type="A">
<li>

```gcloud projects undelete project1```</li><li>

```gcloud projects restore project1```</li><li>

```gcloud projects revert project1```</li>
<li>There is no option to undo this action</li>
</ol> 

<br>

<ins>Correct answer: A</ins>

For further information on how to recover a deleted project, visit the
following link:<br>
<https://cloud.google.com/sdk/gcloud/reference/projects/undelete><br>

##

48. Which method would be the most optimal for creating 15 independent
    Compute Engine VMs with the same settings?<br><br>

<!-- -->

<ol type="A">
<li>In the <b>Compute Engine</b> view, go to the <b>VM instances</b> section
    and select the <b>BULK CREATE VMs</b> option</li>
<li>Create an instance template and use a managed instance group to
    deploy the required number of VMs</li>
<li>Use bulk creation in the CLI – for example, <code>gcloud compute instances bulk create --name-pattern=vm## --count=15 --zone=europe-central2-a --network=my-vpc-network --subnet=warsaw-subnet</code></li>
<li>Use bulk creation in the CLI – for example, <code>gcloud compute instances bulk create --predefined-names=vm1,vm2,vm3,vm4,.. --zone=europe-central2-a --network=my-vpc-network --subnet=warsaw-subnet</code></li>
</ol> 

<br>

<ins>Correct answer: C</ins>

For further information on create multiple Compute Engine virtual
machines and name pattern generation, visit the following link:<br>
<https://cloud.google.com/sdk/gcloud/reference/compute/instances/bulk/create><br>

##

49. In which case is using a Pub/Sub Push subscription type as a
    delivery mechanism for an application the best option?<br><br>

<!-- -->

<ol type="A">
<li>When you’re dealing with a large volume of messages</li>
<li>When high message throughput is expected</li>
<li>When Google Cloud credentials can’t be used</li>
<li>When a public HTTPS endpoint with a non-self-signed certificate
    can’t be used</li>
</ol>  

<br>

<ins>Correct answer: C</ins>

When dealing with a large volume of messages, high throughput, and HTTPs
public endpoints that have non-self-signed certificates, pull
subscription is the way to go. If Google Cloud credentials cannot be
utilized, then push subscription is recommended instead.

Check out the following link for a comparison table between Pub/Sub push
and pull subscription types:<br>
<https://cloud.google.com/pubsub/docs/subscriber##subscription_type_comparison><br>

##

50. You want to provide internet access to your Compute Engine VMs,
    which are deployed in two zones – <code>europe-west3</code> and <code>europe-central2</code> –
    in the same VPC (my-vpc) in a newly created project called
    <code>my-project</code>. Which set of commands should you run?<br><br>

<!-- -->
<ol type="A">
<li>

```
gcloud compute routers create router-waw --project=my-project --network=my-vpc --region=europe-central2

gcloud compute routers create router-fra --project=my-project --network=my-vpc --region=europe-west3

gcloud compute routers nats create nat-waw --router=router-waw --region=europe-central2 --auto-allocate-nat-external-ips --nat-all-subnet-ip-ranges

gcloud compute routers nats create nat-fra --router=router-fra --region=europe-west3 --auto-allocate-nat-external-ips --nat-all-subnet-ip-ranges
```
</li>
<li>

```
gcloud compute routers create router my-router –project=my-project --network=my-vpc

gcloud compute routers nats create nat –router=my-router --auto-allocate-nat-external-ips --nat-all-subnet-ip-ranges
```
</li>
<li>

```
gcloud compute routers create router my-router --project=my-project --network=my-vpc

gcloud compute routers nats create nat-waw --router=my-router --region=europe-central2 --auto-allocate-nat-external-ips --nat-all-subnet-ip-ranges

gcloud compute routers nats create nat-fra --router=my-router --region=europe-west3 --auto-allocate-nat-external- ips --nat-all-subnet-ip-ranges 
```

</li>
<li>
Compute Engine VMs are always created with a public IP, allowing
    internet egress with no additional configuration
</li>
</ol>

<br>

<ins>Correct answer: A</ins>

Before creating Cloud NAT, it is necessary to first create Cloud Router.
It's important to note that both of these services are regional and must
be created for each location.

To learn more about the steps required to create Cloud Router and Cloud
NAT, please visit the following links:<br> 
<https://cloud.google.com/network-connectivity/docs/router/how-to/create-router-vpc-network##create_a><br>
<https://cloud.google.com/nat/docs/set-up-manage-network-address-translation##set_up_a_simple_configuration><br>

##