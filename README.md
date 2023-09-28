# Hyper-V Terraform Automation 🚀

Automate the creation and management of Hyper-V resources using Terraform. This project uses the `taliesins/hyperv` provider.

## Requirements 📋

- Terraform v1.x
- Hyper-V enabled on your machine
- `taliesins/hyperv` Terraform provider

## How It Works 🛠

### Terraform Provider Setup

This project uses the `taliesins/hyperv` provider with version `1.0.4`.

### Hyper-V Network Switch 🌐

Creates a Hyper-V network switch with the name `Access_to_LAN`. It's an external switch with no special embedded teaming or IOV configurations.

### Hyper-V Machine Instance 🖥

Creates a Hyper-V machine instance named `Kubernetes_UbuntuLTS` with the following specs:
- Memory: 3GB to 6GB
- Processor Count: 6 CPUs

## How to Run 🏃

1. **Initialize Terraform**
    ```bash
    terraform init
    ```
2. **Apply Configuration**
    ```bash
    terraform apply
    ```

## Optional Features (Commented Out) 🎛

- **DMZ Network Switch**: An internal network switch configuration is available but commented out.
- **VM Firmware**: VM firmware options including boot order are available but commented out.
- **Cloud-Init**: Cloud-init configuration is available but commented out.
- **Provisioner**: A local-exec provisioner to attach ISO and set boot order is available but commented out.

## Note 🚨

Make sure you understand the impact of these configurations on your Hyper-V setup.

