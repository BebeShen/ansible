# ansible

ansible playground

## Usage

* `ping.yml`: ping DUTs
    ```shell
    ansible-playbook playbooks/ping.yml
    ```
* `build.yml`: build code
    ```shell
    ansible-playbook playbooks/build.yml --extra-vars "code_dir=<code_dir_name>"
    # example: build basic_connection program
    ansible-playbook playbooks/build.yml --extra-vars "code_dir=basic_connection"
    ```
* `runswd.yml`: run switchd
    ```shell
    ansible-playbook playbooks/runswd.yml 
    ```