[![Docker Repository on Quay](https://quay.io/repository/aaroc/fg_db/status?token=6970b0c0-8e27-4269-8f7b-4e26da487ece "Docker Repository on Quay")](https://quay.io/repository/aaroc/fg_db)  [![Build Status](https://travis-ci.org/AAROC/AAROC.fg-db.svg?branch=master)](https://travis-ci.org/AAROC/AAROC.fg-db)

# FutureGateway Data Persistence role (MySQL DB)

Adds a FutureGateway data persistence  service (MySQL database) to your [Ansible Container](https://github.com/ansible/ansible-container) project. Run the following commands
to install the service:

```
# Set the working directory to your Ansible Container project root
$ cd myproject

# Install the service
$ ansible-container install AAROC.fg-db
```

## Requirements

- [Ansible Container](https://github.com/ansible/ansible-container)
- An existing Ansible Container project. To create a project, simply run the following:
    ```
    # Create an empty project directory
    $ mkdir myproject

    # Set the working directory to the new directory
    $ cd myproject

    # Initialize the project
    $ ansible-contiainer init
    ```

- Continue listing any prerequisites here...


## Role Variables

Most variables are set in `default/main.yml` and `vars/main.yml` :

  * `mysql_port`: Port on which MySQL database server is listening
  * `fg_user`: username on the API server allowed to connect to the database.
  * `fg_db_user`: usernmae in the DB granted access to the DB.
  * `fg_db_name`: Name of the database in the DB server used by the API server to write events
  * fg_db_schemaver: Version number of the database schema
  * `db_prerequisites`: OS-dependent list of prerequisite system packages
  * `python_mysql`: OS-dependent name of the mysql python interface package

## Dependencies

none

## License

BSD

## Author Information

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
