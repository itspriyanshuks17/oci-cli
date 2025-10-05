# 🧭 Oracle Cloud Infrastructure (OCI) CLI — Installation Guide (2025)

The **Oracle Cloud Infrastructure (OCI) Command Line Interface (CLI)** is a powerful tool that enables users to manage OCI resources directly from the terminal. Below are the official installation steps for **Windows**, **Linux**, and **macOS** systems.

---

## 🪟 Windows Installation

You can install the OCI CLI on Windows using either the **MSI installer** or **PowerShell**.

### **Option 1: Using MSI Installer**

1. Download the latest **MSI installer** from the [Oracle GitHub OCI CLI Releases Page](https://github.com/oracle/oci-cli/releases).
2. Run the installer and follow the on-screen instructions.

### **Option 2: Using PowerShell**

1. Open **PowerShell** as **Administrator**.
2. Run the following commands:

   ```powershell
   Set-ExecutionPolicy RemoteSigned
   Invoke-WebRequest https://raw.githubusercontent.com/oracle/oci-cli/master/scripts/install/install.ps1 -OutFile install.ps1
   iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/oracle/oci-cli/master/scripts/install/install.ps1'))
   ```
3. After installation, verify by running:

   ```powershell
   oci --version
   ```

---

## 🐧 Linux and <img width="1" height="2" alt="image" src="https://github.com/user-attachments/assets/cec078e6-b9bc-47bd-9265-40446b7de95a" />
 macOS Installation

### **Linux (All Major Distributions)**

Run the following command in your terminal:

```bash
bash -c "$(curl -L https://raw.githubusercontent.com/oracle/oci-cli/master/scripts/install/install.sh)"
```

To automatically accept all defaults:

```bash
bash -c "$(curl -L https://raw.githubusercontent.com/oracle/oci-cli/master/scripts/install/install.sh)" --accept-all-defaults
```

### **macOS (via Homebrew)**

If you have Homebrew installed, simply run:

```bash
brew install oci-cli
```

---

## 🧩 Other Environments

* **Oracle Linux Cloud Developer Images** and **Autonomous Linux** may already include the OCI CLI pre-installed.
* For **offline installations**, download the ZIP file from [OCI CLI Releases on GitHub](https://github.com/oracle/oci-cli/releases), unzip it, and run the install script corresponding to your operating system.

---

## ✅ Verifying the Installation

Once the installation is complete, confirm the CLI is working by running:

```bash
oci --version
```

You should see an output similar to:

```
3.x.x
```

---

## 📚 References

1. [Oracle Docs: Install the CLI](https://docs.oracle.com/en-us/iaas/Content/API/SDKDocs/cliinstall.htm)
2. [Oracle Docs: CLI Concepts](https://docs.oracle.com/en-us/iaas/Content/API/Concepts/cliconcepts.htm)
3. [OCI CLI GitHub Repository](https://github.com/oracle/oci-cli)
4. [Installing OCI CLI on Oracle Linux](https://www.geraldonit.com/installing-the-oracle-cloud-infrastructure-cli-on-oracle-linux-8/)
5. [Manual (Offline) Installation Guide](https://docs.public.content.oci.oraclecloud.com/en-us/iaas/Content/API/SDKDocs/climanualinst.htm)
6. [YouTube: OCI CLI Installation Tutorial](https://www.youtube.com/watch?v=rEHwcJdRf8M)
7. [How to Configure OCI CLI in Windows](https://oracleshare.com/configure-oracle-oci-command-line-interface-cli-in-windows/)
8. [Advanced OCI CLI Commands (Dev.to)](https://dev.to/farisdurrani/advanced-oci-cli-syntax-and-commands-4hpp)
9. [OCI CLI Official Documentation](https://docs.oracle.com/iaas/tools/oci-cli/latest/oci_cli_docs/)
10. [SkillBuilders — OCI CLI Configuration Steps](https://skillbuilders.com/6-steps-to-install-and-configure-oci-cli/)
