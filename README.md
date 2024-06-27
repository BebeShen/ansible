# ansible

ansible playground

## Usage

* `ping.yml`: ping DUTs
    ```shell
    ansible-playbook playbooks/ping.yml
    ```
* `build.yml`: build code
    ```shell
    ansible-playbook playbooks/build.yml --extra-vars "program=<program_name>"
    # example: build basic_connection program
    ansible-playbook playbooks/build.yml --extra-vars "program=basic_connection"
    ```


    > Note: `192.168.30.21`這台一直有sde加載不到的問題，故目前請手動 build 之


* `runswd.yml`: run switchd
    ```shell
    ansible-playbook playbooks/runswd.yml 
    ```

* `path*_test.yml`: testing path/topology
    ```shell
    ansible-playbook playbooks/path*_test.yml --extra-vars "path=<path> program=<program_name>"
    # example
    ansible-playbook playbooks/path*_test.yml --extra-vars "path=path3 program=basic_connection"
    ```
