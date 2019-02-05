### About
Project created for _Computer System Administration_ classes.

### Project overview
* **Ansible** automation
* **Nginx** with **load balancer** and **proxy pass** configuration
* **TIG** pack - **Telegraf, InfluxDB and Grafana** with fully featured **dashboard**
* **Systemd service** to run **Java (Spring)** application 
* **Let's Encrypt** auto configuration

### How to use
* Default password for Ansible Vault was set to "**student1**"
* Default credentials for Grafana: "**admin:admin**"
* `group_vars` include predefined vars for necessary packages URLs
* Prepare machines for hosts groups:
    * Nginx machine
    * two machines for running application
    * machine for statistics
* Set variables values in `hosts.ini`
* Put your `*.jar` file into `app/roles/files`
* Run `ansible-playbook --ask-vault-pass --extra-vars "app_name=YOUR_APP_NAME" infrastructure.yml`
* Tested on **Amazon EC2 Linux**

### Note:
**This project is no longer maintained!**
