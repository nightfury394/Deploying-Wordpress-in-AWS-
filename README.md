+------------+       +-------------+      +----------------+
|            |       |             |      |                |
|  Local PC  +---->+  EC2 Instance  +---->+   WordPress    |
|            |       |    (AMI)      |    |                |
+------------+       +-------------+      +----------------+
     |                         |                  |
     |      Connect via SSH    |                  |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     |      Install Apache     |                  |
     |      Install PHP        |                  |
     |      Install MySQL      |                  |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     |     Download WordPress  |                  |
     |     Extract to web root |                  |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     |     Create MySQL DB     |                  |
     |     Create MySQL user   |                  |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     |   Edit WordPress config |                  |
     |   to use MySQL DB/user  |                  |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     | Access WordPress via    |                  |
     | public IP of EC2        |                  |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     | Complete WordPress      |                  |
     | installation process    |                  |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     | (Optional) Set up domain|                  |
     |  name and create CNAME  |                  |
     |  record                  |                 |
     |                         |                  |
     +-------------------------+                  |
     |                         |                  |
     | (Optional) Set up SSL/TLS|                 |
     |  using Let's Encrypt    |                  |
     |                         |                  |
     +-------------------------+                  |
