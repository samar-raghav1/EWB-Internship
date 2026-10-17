# Project Setup – Day 1 Summary

On Day 1, I focused on building the foundational network architecture:

- **Created two VPCs** (VPC A and VPC B) with public and private subnets.
- **Configured a bastion host** in VPC A’s public subnet for secure access.
- **Set up private subnets** for application instances in both VPCs.
- **Established a VPC peering connection** between VPC A and VPC B.
- **Defined route tables** to enable communication across subnets and VPCs.
- **Created security groups**:
  - Bastion SG allowing inbound SSH from my local machine.
  - Private EC2 SGs allowing inbound SSH from the bastion subnet CIDR.
- **Tested connectivity**:
  - Verified SSH access into the bastion host.
  - Prepared for SSH access into private EC2s via bastion.

This completes the initial networking and access setup, laying the groundwork for secure communication between resources across both VPCs.


##  Testing Commands

### 1. SSH into Bastion (from local laptop)
**Syntax:**
```bash
ssh -i <bastion-key.pem> ubuntu@<bastion-public-ip>

2.COPY PEM key into bastion
scp -i <bastion-key.pem> <local-pem-file> ubuntu@<bastion-public-ip>:/home/ubuntu/

3.SH into Private EC2 (from Bastion)
ssh -i <private-key.pem> ubuntu@<private-ec2-private-ip>

4.Ping Private EC2 (from Bastion)
ping <private-ec2-private-ip>

```

**Day 1 achievements** and provides **copy‑paste‑ready commands** for testing.