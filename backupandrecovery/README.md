# kubernetes Backup and Recovery using CronJobs and Azure FileShare   


This solution will provide backup mechnism for you postgres(Can choose any database) database. 
Using cron job you could schedule the script to run at certain time interval. 
Script will publish the backup on kubernetes volumes and then to azure storage. 