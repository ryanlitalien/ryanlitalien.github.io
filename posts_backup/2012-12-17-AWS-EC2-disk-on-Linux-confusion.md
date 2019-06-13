---
layout: post
title: AWS EC2 disk on Linux confusion
published_at: 2012-12-17
tags:
  - Technology
  - AWS
---

After our instance store instance had issues, we converted it to an EBS store.  So according to the AWS documentation, you have to mount the partition to the filesystem. The AWS docs are a bit heavy, so for a quick reference:

AWS console: `/dev/sdf +`
Linux console: `/dev/xvdf`

These are the same partitions, just different names.

AWS Docs: [http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-attaching-volume.html](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-attaching-volume.html)

Great how-to: [http://maplpro.blogspot.com/2012/05/how-to-mount-ebs-volume-into-ec2-ubuntu.html](http://maplpro.blogspot.com/2012/05/how-to-mount-ebs-volume-into-ec2-ubuntu.html)
