#####Study Material
=======================================================================
#####Question1
![Question1](/images/ops1.gif)
#####Answer: **C** 
#####Comment: 
>This is a sucky question, in my experience the volume cannot be detached when you are making a snapshot But I suspect that might have been unexpected behviour I experienced, that answer is **C**.

========================================================================
#####Question2
![Question2](/images/ops2.gif)
------------------------------------------------------------------------
#####Answer: D 
> an alias record is the right answer, per:
![Question2a](/images/ops2a.png)

> http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resource-record-sets-choosing-alias-non-alias.html

=========================================================================
#####Question3
![Question3](/images/ops3.gif)
#####Answer: A 
#####Comment: 
>A is simple and doable, I can't find any mention of "SNMP" in the Cloudwatch developers guide, seems like a dumb way to go about it, if not impossible

=========================================================================
#####Question4
![Question4](/images/ops4.gif)
#####Answer: A, D
#####Comment: 
>C and E are both false

=========================================================================
#####Question5
![Question5](/images/ops5.gif)
#####Answer: A, D
#####Comment: 
>C is wrong, the only thing needed besides NACLs and SG's to allow the traffic is the local route in the route table.

=========================================================================
#####Question6
![Question6](/images/ops6.gif)
#####Answer: Should be A, B, C
#####Comment: 
>x.509 certs are listed in the Operational Checklists pdf, but signing certs should be wrong or 2 ambiguous.

=========================================================================
#####Question7
![Question7](/images/ops7.gif)
#####Answer: A, B or C are correct
#####Comment: 
>to make and existing EBS vol PIOPs vol you must make new vols from a snapshot of your original, you can EBS optimize an existing instance, and SSD would be better than magnetic
>, however, PIOPs on a magnetic vol would not be adequate, so you could infer C is completely wrong

=========================================================================
#####Question8
![Question8](/images/ops8.gif)
#####Answer: A, D
#####Comment: 
>Evictions are items moved out of Elasticache to make room for new items,
>GetMisses mean the item requested wasn't in cache, these 2 metrics mean the size is too small /n
>Items in Elasticache are stored on the instance store storage of the instance so total cache is number of Elasticache instances * their ephemeral stores, increase the size.

=========================================================================
#####Question9
![Question9](/images/ops9.gif)
#####Answer: D
#####Comment: 
>D is the only answer that will increase bandwidth - total bandwidth used as there will be more instances

=========================================================================
#####Question10
![Question10](/images/ops10.gif)
#####Answer: B
#####Comment: 
>

=========================================================================
#####Question11
![Question11](/images/ops11.gif)
#####Answer: A, B, C
#####Comment: 
>

=========================================================================
#####Question12
![Question12](/images/ops12.gif)
#####Answer: A, D
#####Comment: 
>

=========================================================================
#####Question13
![Question13](/images/ops13.gif)
#####Answer: D
#####Comment: 
>

=========================================================================
#####Question14
![Question14](/images/ops14.gif)
#####Answer: B, C
#####Comment: 
>

=========================================================================
#####Question15
![Question15](/images/ops15.gif)
#####Answer: D
#####Comment: 
>B could be true as Trusted Advisor will warn you if you are already using %80 of your limit
>and x times 20 = 175 means you currently have 9 instances, it depends on the type if that already
>over the limit or not, some on-demand limits are are low as 2, some are as high as 20.

=========================================================================
#####Question16
![Question16](/images/ops16.gif)
#####Answer: A
#####Comment: 
>

=========================================================================
#####Question17
![Question17](/images/ops17.gif)
#####Answer: A, D
#####Comment: 
>

=========================================================================
#####Question18
![Question18](/images/ops18.gif)
#####Answer: A, D
#####Comment: 
>

=========================================================================
#####Question19
![Question19](/images/ops19.gif)
#####Answer: C
#####Comment: 
>http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ComponentsAMIs.html


=========================================================================
#####Question20
![Question20](/images/ops20.gif)
#####Answer: A, B, D
#####Comment: 
>no evidence on my answer

=========================================================================
#####Question21
![Question21](/images/ops21.gif)
#####Answer: A, B
#####Comment: 
>

=========================================================================
#####Question22
![Question22](/images/ops22.gif)
#####Answer: B
#####Comment: THere is no IGW config beyond attach/detach
>

=========================================================================
#####Question23
![Question23](/images/ops23.gif)
#####Answer: A, D
#####Comment: 
>Individual Amazon S3 objects can range in size from 1 byte to 5 terabytes. The largest object that can be uploaded in a single PUT is 5 gigabytes. For objects larger than 100 megabytes, customers should consider using the Multipart Upload capability.
>
>A is correct
>B is ridiculous
>C is technically wrong, but the term "virtually" is a bit of a concern
>D seems more correct than C
>E is wrong

=========================================================================
#####Question24
![Question24](/images/ops24.gif)
#####Answer: B
#####Comment: 
>

=========================================================================
#####Question25
![Question25](/images/ops25.gif)
#####Answer: A
#####Comment: 
>

=========================================================================
#####Question26
![Question26](/images/ops26.gif)
#####Answer: C
#####Comment: 
>

=========================================================================
#####Question27
![Question27](/images/ops27.gif)
#####Answer: A, B, 
#####Comment: 
>

=========================================================================
#####Question28
![Question28](/images/ops28.gif)
#####Answer: 
#####Comment: 
>

=========================================================================
#####Question29
![Question29](/images/ops29.gif)
#####Answer: A
#####Comment: 
>

=========================================================================
#####Question30
![Question30](/images/ops30.gif)
#####Answer: D 
#####Comment: 
>I say CF as it says manage "infrastructure"

=========================================================================
#####Question31
![Question31](/images/ops31.gif)
#####Answer: C
#####Comment: 
>THe answer is A or C, a very few couple of people mention you could have 2 ELBs
>

=========================================================================
#####Question32
![Question32](/images/ops32.gif)
#####Answer: A
#####Comment: 
>I see no reason you can't do snapshots

=========================================================================
#####Question33
![Question33](/images/ops33.gif)
#####Answer: A
#####Comment: 
>C can be done easily with Cloudwatch
>[AWS Link](https://aws.amazon.com/about-aws/whats-new/2013/01/08/use-amazon-cloudwatch-to-detect-and-shut-down-unused-amazon-ec2-instances/)
>

=========================================================================
#####Question34
![Question34](/images/ops34.gif)
#####Answer: A
#####Comment: 
>I don't know, maybe C - more to follow

=========================================================================
#####Question35
![Question35](/images/ops35.gif)
#####Answer: D
#####Comment: 
>

=========================================================================
#####Question36
![Question36](/images/ops36.gif)
#####Answer: B
#####Comment: 
>this is worded badly and there is an agent you can load on Ubuntu and Amazon Linux that will capture
>"disk" or partition usage metrics

=========================================================================
#####Question37
![Question37](/images/ops37.gif)
#####Answer: B
#####Comment: 
>

=========================================================================
#####Question38
![Question38](/images/ops38.gif)
#####Answer: C, D
#####Comment: 
>

=========================================================================
#####Question39
![Question39](/images/ops39.gif)
#####Answer: B
#####Comment: 
>Chef and Beanstalk work great together, but answer B seems awful simplistic, not mentioning where Chef is configured/stood up. Chef and Beanstalk should "minimize the administrative burden", so B is the strongest answer
>Further, the Opsworks FAQ indicates Beanstalk has a more narrow list of available architectural options, to make Beanstalk the simpler solution. 
>http://gabrielsomoza.com/aws/case-for-opsworks/

=========================================================================
#####Question40
![Question40](/images/ops40.gif)
#####Answer: B
#####Comment: 
>There are no deny rules for SGs, must be NACLs

=========================================================================
#####Question41
![Question41](/images/ops41.gif)
#####Answer: B
#####Comment: 
>

=========================================================================
#####Question42
![Question42](/images/ops42.gif)
#####Answer: C
#####Comment: 
>

=========================================================================
#####Question43
![Question43](/images/ops43.gif)
#####Answer: A
#####Comment: 
>

=========================================================================
#####Question44
![Question44](/images/ops44.gif)
#####Answer: B
#####Comment: 
>You end up having both an EC2 Instance health check and an ELB health check. Coincidentally this link is one of the few mentions of multiple ELBs fronting the same instances,
>which is alluded to in an earlier question on redundancy. When you have multiples all ELBs must report an instance as InService or it gets crushed.
> http://docs.aws.amazon.com/AutoScaling/latest/DeveloperGuide/as-add-elb-healthcheck.html

=========================================================================
#####Question45
![Question45](/images/ops45.gif)
#####Answer: C
#####Comment: 
>

=========================================================================
#####Question46
![Question46](/images/ops46.gif)
#####Answer: C
#####Comment: 
>

=========================================================================
#####Question
![Question](/images/ops.gif)
#####Answer: testing a push 
#####Comment: 
>
=========================================================================
#####Question
![Question](/images/ops.gif)
#####Answer: 
#####Comment: 
>
=========================================================================
#####Question
![Question](/images/ops.gif)
#####Answer: 
#####Comment: 
>
=========================================================================
#####Question
![Question](/images/ops.gif)
#####Answer: 
#####Comment: 
>
