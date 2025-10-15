Gnetcli
======
The ultimate solution for CLI automation in Golang. It provides a universal way to execute arbitrary commands using a CLI, eliminating the need for screen scraping with expect.
The project consist of go-library, GRPC server and CLI tool. It is typically used for automating network equipment such as Cisco, Juniper, Huawei, etc.

## Feature Overview:
* **Execute commands instead of just reading and writing.**
* **Pager, questions and error handling are supported.**  
  Describe CLI interface in a few expressions and get full power of the project.
* **The project supports several network vendors, including Huawei, Juniper, Cisco, and RouterOS.**
* **Netconf is supported.**  
  Exec netconf in same manner as text command to simplify automation workflow.
* **SSH tunneling is supported.**
* **Clean output**  
  Evaluation of terminal control codes and removal of echoes.
