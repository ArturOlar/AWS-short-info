### EC2 Instance Store

EC2 Instance Store is not an **EBS**, it's different kind of storage. It's a local, physical storage that attached to EC2
instance, and because this is a physical storage, it works faster than **EBS**, because **EBS** is a network driver.

- EBS volumes are network drives with good but “limited” performance
- If you need a high-performance hardware disk, use **EC2 Instance Store**
- Better I/O performance
- EC2 Instance Store lose their storage if they’re stopped (ephemeral)
- Good for buffer / cache / scratch data / temporary content
- Risk of data loss if hardware fails
- Backups and Replication are your responsibility