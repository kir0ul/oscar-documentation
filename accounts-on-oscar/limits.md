---
title: Account Limits
date: '2019-01-31 22:01:46 +0000'
project: Oscar
section: Accounts
icon: check
---

# Account Limits

## Account Limits

{% hint style="info" %}
The number and size of jobs allowed on Oscar vary with both partition and type of user account. You can email support@ccv.brown.edu if you need advice on which partitions to use
{% endhint %}

The following partitions are available to all Oscar users:

| Name | Purpose |
| :--- | :--- |
| batch | general purpose computing |
| debug | short wait time, short run time partition for debugging |
| gpu | GPU nodes |
| gpu-debug | short wait time, short run time partition for gpu debugging |
| bigmem | large memory nodes |
| smp | older large memory nodes |

## batch partition

* General purpose computing
* Priority is determined by account type \(from highest

  to lowest: condo, premium, exploratory\)

| Resource Limit | Exploratory \(free\) Account | Premium Account | Condo |
| :--- | :--- | :--- | :--- |
| Maximum number of cores in use at once | 16 | 208 | condo size |
| Maximum number of jobs | 16 | 208 | condo size |
| Maximum memory in use at once \(GB\) | 123 | 1024 | condo size |
| Limit, sum of all jobs \(core•minutes\) | 46,100 | 998,400 | condo size |

Condo limits apply to the group \(i.e., they reflect the sum of all users on the condo\). Condo users can check the limits on their condo with the command `condos`.

{% hint style="warning" %}
There is no limit on the time for condo jobs, but users should be aware that planned maintenance on the machine may occur \(one month’s notice is given prior to any planned maintenance\).
{% endhint %}

## debug partition

* Short wait time, short run time access for debugging
* All users have the same limits and priority on the debug partition

| Resource Limit | All Users |
| :--- | :--- |
| Maximum number of cores in use at once | 16 |
| Maximum number of jobs | 2 |
| Maximum memory in use at once \(GB\) | 123 |
| Limit, sum of all jobs \(minutes\) | 30 |

## gpu partition

* For GPU-based jobs
* Premium users get higher priority and more resources than free users on the GPU partition
* Condo users submit to the gpu partition with normal or priority access \(if they have a priority account in addition to their condo\)

| Resource Limit | Exploratory \(free\) Account | Premium Account |
| :--- | :--- | :--- |
| Maximum number of GPUs in use at once | 2 | 8 |
| Maximum number of CPUs in use at once | 4 | 16 |
| Maximum memory in use at once \(GB\) | 46 | 180 |
| Limit, sum of all jobs \(GPU•hours\) | 48 | 192 |

## gpu-debug partition

* Short wait time, short run time gpu access for debugging
* All users have the same limits and priority on the gpu-debug partition

| Resource Limit | All Users |
| :--- | :--- |
| Maximum number of GPUs in use at once | 1 |
| Maximum number of CPUs in use at once | 2 |
| Maximum memory in use at once \(GB\) | 23 |
| Limit, sum of all jobs \(GPU•hours\) | 4 |

## bigmem

* For jobs requiring large amounts of memory
* Premium users get higher priority and more resources than free users on the bibmem partition
* Condo users submit to the bigmem partition with normal or priority access \(if they have a priority account in addition to their condo\)

| Resource Limit | Exploratory \(free\) Account | Premium Account |
| :--- | :--- | :--- |
| Maximum number of jobs | 1 | 2 |
| Maximum memory in use at once \(GB\) | 750 | 750 |
| Time limit \(wall clock\) per job \(hours\) | 24 | 96 |
| Limit, sum of all jobs \(core•minutes\) | 46,080 | 184,320 |

## smp partition

* For jobs requiring large amounts of memory
* Premium users get higher priority and more resources than free users on the SMP partition
* Condo users submit to the SMP partition with normal or priority access \(if they have a priority account in addition to their condo\)

| Resource Limit | Exploratory \(free\) Account | Premium Account |
| :--- | :--- | :--- |
| Maximum number of jobs | 1 | 2 |
| Maximum memory in use at once \(GB\) | 503 | 1006 |
| Time limit \(wall clock\) per job \(hours\) | 24 | 48 |
| Limit, sum of all jobs \(core•minutes\) | 92,160 | 184,320 |
