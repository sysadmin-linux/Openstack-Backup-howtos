# Backup process flow:
1. Pause VM
2. Detach Storage Volume from respective VMs
3. Snapshot VM store on Glance
4. Call Cinder backup APIs to back up Storage Volume  to Swift
5. Keep track of these copies in an Excel sheet
6. Attach Storage Volume back to VM
7. Resume VM
# show disk quota
openstack project show -c <ID> -f value <PROJ.NAME> 
cinder quota-usage <PROJ.ID>
# Configure cinder CLI backup
https://www.server-world.info/en/note?os=CentOS_7&p=openstack_train2&f=12
# Backup your Virtual MAchines in OpenSTACK
https://itgix.com/blog/backing-up-your-virtual-machines-in-openstack/
# Back up and restore volumes and snapshots
https://docs.openstack.org/newton/admin-guide/blockstorage-volume-backups.html
# Understanding, using, and managing the Block Storage backup service in OpenStack
https://access.redhat.com/documentation/en-us/red_hat_openstack_platform/16.1/html-single/block_storage_backup_guide/index
# OpenStack: Quick and automatic instance snapshot backup and restore (and before an apt upgrade) with nova backup
https://raymii.org/s/tutorials/OpenStack_Quick_and_automatic_instance_snapshot_backups.html
# cinderback
https://kandi.openweaver.com/python/Akrog/cinderback
# Dude, where's my volume? A guide to storage backup, migration, and replication with OpenStack Cinder
https://www.youtube.com/watch?v=ahTQXaz5-VI
# Cinder Backup/Restore with Horizon
https://support.binero.com/knowledge-base/cinder-backup/?lang=en
# Install OPENSTACK easy with DEVSTACK
https://docs.openstack.org/devstack/latest
# Something maybe not useful
https://stackoverflow.com/questions/53969104/shell-script-to-wait-till-the-command-execute-and-status-change
