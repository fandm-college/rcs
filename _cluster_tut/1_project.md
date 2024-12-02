---
layout: page
title: Introduction to the compute cluster 
img: assets/img/compute.jpg
importance: 1
---
 A compute cluster is a set of interconnected computers that work together
 as if they were one very large computer.  The F&M compute cluster consists of

 - 1 head node
    - Not accessible to user or for computation
    - Handles the behind the scenes cluster management
 - 1 submit node 
    - User access for copying data and job submission
    - Not usable for computation
 - 36 compute nodes each with
    -  40 CPUs
    - 192 GB of memory
- 2 GPU nodes
    - 4 GPUs each
    - Node g01 has 40 CPUs and 192 GB
    - Node g02 has 64 CPUs and 500 GB of memory
- 18TB of drive storage **shared among all users**

## Performing computations

A fairly typical research workflow for the cluster is as follows:

1. Copy data to the cluster
2. Create a file (henceforth referred to as a job script) with details
   about compute resources and your software
3. Submit your job script to run your computations
4. When computations finish, copy data/results off the cluster for 
   post-processing and analysis.

Running your software on a compute cluster is different from how you run software on your personal computer.
The F&M cluster uses a software package called **Slurm** (**S**imple **l**inux **u**tility for
**r**esource **m**anagement) which controls how and when your software is run.  Basically, you 
create a file that requests resources like number of CPUs and amount of memory, and provides details
about the software you want to use.  Slurm uses that information to add your request to a job
queue.  Your job will run when

1. Your job gets to or near the top of the job queue AND
2. All necessary compute resources (e.g., CPUs, memory, etc.) you requested become available

## Requesting resources

Exact details for specifying in your job script are covered ???.  Here we discuss some guidelines
for how many resources to request.  Requesting an appropriate amount of resources is important
because it has a direct impact on when jobs can start running and how many jobs can be running at 
the same time on the cluster.

> [!NOTE]
> When you request compute resources in your job script, those resources are reserved for
> your job **whether your job uses them or not**.  That means that if your request too much
> of a resource, that resource is wasted in the sense it could have been used by another 
> job waiting to be run. \ 
> When it comes to the amount of resources you request, we aren't asking that you request 
> the exact right number of resources because there aren't necessarily exact right 
> values.  What we are asking is, to the extent possible, you don't grossly 
> over-request resources for your jobs.

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
