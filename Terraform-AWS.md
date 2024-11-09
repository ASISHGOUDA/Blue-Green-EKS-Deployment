
# Installation Guide for AWS CLI and Terraform

This guide provides instructions for installing the AWS CLI and Terraform on a Linux system.

---

### Prerequisites

Ensure you have the necessary tools installed:

- `curl`: For downloading files from the internet.
- `unzip`: For extracting files.

To install these tools, run:

```bash
sudo apt update && sudo apt install -y curl unzip
```

---

### Installing Terraform

To install Terraform, use the following commands:

1. Download the latest Terraform package:

   ```bash
   curl -fsSL "https://releases.hashicorp.com/terraform/1.9.8/terraform_1.9.8_linux_amd64.zip" -o terraform.zip
   ```

2. Unzip the downloaded file:

   ```bash
   unzip -o terraform.zip
   ```

3. Move the `terraform` binary to `/usr/local/bin` for global access:

   ```bash
   sudo mv terraform /usr/local/bin/
   ```

4. Remove the downloaded zip file:

   ```bash
   rm terraform.zip
   ```

5. Verify the installation:

   ```bash
   terraform -v
   ```

---

### Installing AWS CLI

To install the AWS CLI, use the following commands:

1. Download the AWS CLI installation package:

   ```bash
   curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
   ```

2. Unzip the downloaded file:

   ```bash
   unzip awscliv2.zip
   ```

3. Run the installer:

   ```bash
   sudo ./aws/install
   ```

4. Verify the installation:

   ```bash
   aws --version
   ```

5. Remove the installation files:

   ```bash
   rm -rf awscliv2.zip aws
   ```

---

### Configuring AWS CLI

After installing the AWS CLI, configure it using the following command:

```bash
aws configure
```

This command will prompt you to enter your:

- **AWS Access Key ID**
- **AWS Secret Access Key**
- **Default region name**
- **Default output format**

Follow the prompts to complete the configuration.

---

You now have both the AWS CLI and Terraform installed and ready to use!