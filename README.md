To download and install the Oracle Cloud Infrastructure (OCI) CLI, follow these official steps, which vary depending on your operating system:[1][2][3]

### Windows Installation
- Use the MSI installer or PowerShell.
    - With MSI: Download from Oracle's GitHub releases and run the installer.[1]
    - With PowerShell: Open PowerShell as administrator, run:
      ```powershell
      Set-ExecutionPolicy RemoteSigned
      Invoke-WebRequest https://raw.githubusercontent.com/oracle/oci-cli/master/scripts/install/install.ps1 -OutFile install.ps1
      iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/oracle/oci-cli/master/scripts/install/install.ps1'))
      ```
- After installation, verify with:
  ```
  oci --version
  ```


### Linux and macOS Installation
- For most Linux distributions, run:
  ```
  bash -c "$(curl -L https://raw.githubusercontent.com/oracle/oci-cli/master/scripts/install/install.sh)"
  ```
  - To accept all defaults silently, add: `--accept-all-defaults`.[3][1]

- For macOS with Homebrew:
  ```
  brew install oci-cli
  ```


### Other Environments
- Oracle Linux Cloud Developer images and Autonomous Linux may have it pre-installed.[2][4]
- For offline installation, download a ZIP from GitHub OCI CLI releases, unzip, and run the install script for your OS.[5][3]

### Verifying the Installation
- After the installation, confirm by running:
  ```
  oci --version
  ```


These methods cover the standard download and setup for all major operating systems. Oracle’s official docs provide further troubleshooting tips and configuration guides if needed.[2][3][1]

[1](https://docs.oracle.com/en-us/iaas/Content/API/SDKDocs/cliinstall.htm)
[2](https://docs.oracle.com/en-us/iaas/Content/API/Concepts/cliconcepts.htm)
[3](https://github.com/oracle/oci-cli)
[4](https://www.geraldonit.com/installing-the-oracle-cloud-infrastructure-cli-on-oracle-linux-8/)
[5](https://docs.public.content.oci.oraclecloud.com/en-us/iaas/Content/API/SDKDocs/climanualinst.htm)
[6](https://www.youtube.com/watch?v=rEHwcJdRf8M)
[7](https://oracleshare.com/configure-oracle-oci-command-line-interface-cli-in-windows/)
[8](https://www.youtube.com/watch?v=bY3jQMMHxdw)
[9](https://dev.to/farisdurrani/advanced-oci-cli-syntax-and-commands-4hpp)
[10](https://docs.oracle.com/en-us/iaas/Content/API/SDKDocs/cliconfigure.htm)
[11](https://docs.oracle.com/iaas/tools/oci-cli/latest/oci_cli_docs/)
[12](https://help.okta.com/oag/en-us/content/topics/access-gateway/deploy-oci-cli.htm)
[13](https://database-heartbeat.com/2022/09/26/oci-cli-virtual-environment/)
[14](https://learn.arm.com/install-guides/oci-cli/)
[15](https://www.youtube.com/watch?v=vDMnYY_juM4)
[16](https://skillbuilders.com/6-steps-to-install-and-configure-oci-cli/)
[17](https://www.youtube.com/watch?v=jtGad3GSYh0)
[18](https://www.linkedin.com/pulse/how-install-use-oci-cli-mac-os-from-scratch-valentin-lemains)
[19](https://docs.cloud.jpsovereigncloud.jp/en-us/iaas/tools/oci-cli/3.67.0/oci_cli_docs/oci.html)
[20](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
