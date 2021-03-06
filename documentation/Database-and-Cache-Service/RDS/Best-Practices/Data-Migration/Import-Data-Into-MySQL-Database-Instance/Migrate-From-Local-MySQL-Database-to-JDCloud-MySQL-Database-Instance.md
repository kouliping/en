# Data Transferring from Local MySQL to MySQL Service
It mainly explains how to transfer data from the local self-built MySQL to JD Cloud MySQL service. The self-built MySQL requires operations such as daily maintenance, monitoring and backup, while JD Cloud MySQL service spares these operations and only requires user's attention on the use.

## Precautions
* Use a VM as the transmission medium, if to import the data in local MySQL to the MySQL service.
* New MySQL instance is required to share one ***virtual private cloud*** with the VM.
* Ensure the capacity space of the new MySQL instance not smaller than the self-built local MySQL.

## Operation Steps
1. See specific steps of the MySQL service creation in [Create Cloud MySQL Database Instance](to be added).
2. Create a database through the console to ensure that the name of the database to be exported from the local self-built MySQL is also created in the MySQL service. See specific creation steps in [Create Database](to be added).
3. Create a database account via the console, or use the account that created for the MySQL service creation, and then give this account the ***read/write*** authorization for the new database created in step 2. See specific creation steps in [Create Account](to be added).
4. Export the data from the local self-built MySQL to the local and execute the command after completing the creation and initialization of the MySQL service.

    ```
    mysqldump -u User name -p Password --single-transaction --set-gtid-purged=OFF -B Database name > /Path/Outputted file name.sql

    Parameter description
        User name: User name of self-built database.
        Password: Password of self-built database.
        Database name: Fill in database names to be outputted and separate several database names with spaces
    ```
    
5. Start creating a VM after exporting the local self-built MySQL data to the local.
6. See specific steps of VM creation in [Create VM Instance](https://www.jdcloud.com/help/detail/303/isCatalog/1). Pay attention to following matters when creating VM instances.
    * Make sure that VM shares one ***virtual private cloud*** with the MySQL service created in step 1.
    * A new VM needs a **Public IP*** for public network access, otherwise local data files cannot be uploaded to the VM.
    * Make sure that ***Network ACL*** of the subnet where the VM exists, allows the local SSH to connect to the VM.

7. Upload the local data to the VM and execute the command after VM instance creation.

    ```
    scp /Path/Outputted file name.sql User name of virtual machine@Virtual Machine EIP: /Virtual Machine Path

    Parameter description
        User name of virtual machine: User name at the time of creating a virtual machine instance.
        Virtual Machine EIP: EIP address associated with virtual machine.
        Virtual Machine path: Storage path in virtual machine of files uploaded locally.
    ```

8. Zero error prompt indicates that local files are successfully uploaded to the VM, and then users can import the data into the MySQL service and execute the command.

    ```
    mysql -u User name -p Password -h Cloud database domain < /Virtual machine path/Outputted file name.sql

    Parameter description
        User name: User name in actions of step 3
        Password: Corresponding password of the user in actions of step 3
        Database domain: Please view domain of MySQL service in the Details page of instance.
    ```
9. Zero error prompt indicates successful import. You can log in the MySQL service to see if the data has been imported.
