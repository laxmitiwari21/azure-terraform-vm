# 🚀 Azure VM Provisioning with Terraform

This project demonstrates how to provision a **Linux Virtual Machine on Microsoft Azure** using **Terraform**, ideal for beginners targeting **Cloud Engineer** or **DevOps** roles.

---

## 📁 Project Structure
- ├── main.tf # Main Terraform configuration file
- ├── variables.tf # Input variables
- ├── terraform.tfvars # Variable values (Do not commit secrets!)
- ├── outputs.tf # Outputs like public IP
- └── README.md # Project overview and documentation
## 🧰 Tools Used

- 🏗️ **Terraform** v1.x
- ☁️ **Azure** Free Tier
- 💻 **Ubuntu 20.04 LTS** (Linux VM)
- 🔐 Azure Resource Group, Network Interface, NSG, Public IP, Virtual Network

---

## 🚀 What it Deploys

- A **Virtual Network**
- A **Network Security Group (NSG)** with SSH port open
- A **Public IP Address**
- A **Linux Virtual Machine** with SSH access

---

## 🔧 How to Use

### 1. Clone the Repo

```bash
git clone https://github.com/laxmitiwari21/azure-terraform-vm.git
cd azure-terraform-vm
```
### 2. Configure Azure

Login to your Azure account:
```bash
az login
```

### 3. Initialize Terraform
```bash
terraform init
```

### 4. Preview Changes
```bash
terraform plan
```

### 5. Apply Configuration
```bash
terraform apply
```
Enter the admin password when prompted (from terraform.tfvars or input).

## 🔓 Access the VM
After terraform apply, note the public IP output.
```bash
ssh azureuser@<public_ip>
```
## 📌 Clean Up
To avoid charges:
```bash
terraform destroy
```
## 💼 Why This Project?
- ✅ Beginner-friendly
- ✅ Follows Azure best practices
- ✅ Infrastructure-as-Code (IaC) skills
- ✅ Perfect for resume, GitHub portfolio, and interviews
## 📜 License
MIT License
Made with 💻 by Laxmi Tiwari
