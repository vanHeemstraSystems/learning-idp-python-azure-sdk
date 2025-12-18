# Learning IDP: Python Azure SDK

This repository focuses on mastering the Azure SDK for Python to build, manage, and automate Azure infrastructure for Internal Development Platform (IDP) development.

- [References](./REFERENCES.md)

## 🎯 Learning Objectives

By working through this repository, you will:

1. Master Azure authentication patterns with azure-identity
1. Understand Azure SDK architecture and design patterns
1. Implement resource management operations programmatically
1. Work with async/await patterns in Azure SDK
1. Handle errors and exceptions effectively
1. Optimize SDK usage for performance and cost
1. Apply best practices for production-grade code

## 📚 Prerequisites

- Python 3.11 or higher
- Azure subscription with contributor access
- Azure CLI installed and configured
- Basic understanding of Azure services
- Git and GitHub account

## 🗂️ Directory Structure

```
learning-idp-python-azure-sdk/
├── README.md                          # This file
├── REFERENCES.md                      # Links to resources and related repos
├── pyproject.toml                     # Python project configuration
├── requirements.txt                   # Python dependencies
├── requirements-dev.txt               # Development dependencies
├── .python-version                    # Python version for pyenv
├── .gitignore                         # Git ignore patterns
├── .env.example                       # Environment variables template
│
├── docs/
│   ├── concepts/
│   │   ├── 01-azure-sdk-overview.md
│   │   ├── 02-authentication-patterns.md
│   │   ├── 03-sdk-architecture.md
│   │   ├── 04-async-programming.md
│   │   ├── 05-error-handling.md
│   │   └── 06-best-practices.md
│   ├── guides/
│   │   ├── getting-started.md
│   │   ├── authentication-setup.md
│   │   ├── resource-management.md
│   │   ├── async-operations.md
│   │   └── performance-optimization.md
│   └── examples/
│       ├── basic-authentication.md
│       ├── resource-groups.md
│       ├── storage-accounts.md
│       ├── virtual-networks.md
│       └── compute-resources.md
│
├── src/
│   ├── __init__.py
│   │
│   ├── core/
│   │   ├── __init__.py
│   │   ├── authentication.py          # Authentication utilities
│   │   ├── config.py                  # Configuration management
│   │   ├── exceptions.py              # Custom exceptions
│   │   └── logging_config.py          # Logging setup
│   │
│   ├── identity/
│   │   ├── __init__.py
│   │   ├── credential_manager.py      # Credential management
│   │   ├── managed_identity.py        # Managed Identity patterns
│   │   └── service_principal.py       # Service Principal auth
│   │
│   ├── resource_management/
│   │   ├── __init__.py
│   │   ├── resource_groups.py         # Resource Group operations
│   │   ├── subscriptions.py           # Subscription operations
│   │   └── tags.py                    # Tag management
│   │
│   ├── storage/
│   │   ├── __init__.py
│   │   ├── storage_accounts.py        # Storage Account management
│   │   ├── blob_operations.py         # Blob storage operations
│   │   └── file_shares.py             # File share operations
│   │
│   ├── network/
│   │   ├── __init__.py
│   │   ├── virtual_networks.py        # VNet management
│   │   ├── subnets.py                 # Subnet operations
│   │   ├── security_groups.py         # NSG management
│   │   └── public_ips.py              # Public IP management
│   │
│   ├── compute/
│   │   ├── __init__.py
│   │   ├── virtual_machines.py        # VM management
│   │   ├── disks.py                   # Disk operations
│   │   └── availability_sets.py       # Availability set management
│   │
│   ├── container/
│   │   ├── __init__.py
│   │   ├── container_instances.py     # ACI management
│   │   ├── container_registry.py      # ACR operations
│   │   └── kubernetes.py              # AKS management
│   │
│   └── monitoring/
│       ├── __init__.py
│       ├── diagnostics.py             # Diagnostic settings
│       ├── metrics.py                 # Metrics operations
│       └── alerts.py                  # Alert management
│
├── examples/
│   ├── 01_authentication/
│   │   ├── default_credential.py
│   │   ├── service_principal.py
│   │   ├── managed_identity.py
│   │   └── cli_credential.py
│   │
│   ├── 02_resource_groups/
│   │   ├── create_resource_group.py
│   │   ├── list_resource_groups.py
│   │   ├── update_tags.py
│   │   └── delete_resource_group.py
│   │
│   ├── 03_storage/
│   │   ├── create_storage_account.py
│   │   ├── blob_operations.py
│   │   ├── file_share_operations.py
│   │   └── storage_analytics.py
│   │
│   ├── 04_networking/
│   │   ├── create_virtual_network.py
│   │   ├── configure_nsg.py
│   │   ├── setup_load_balancer.py
│   │   └── private_endpoint.py
│   │
│   ├── 05_compute/
│   │   ├── create_vm.py
│   │   ├── vm_extensions.py
│   │   ├── managed_disks.py
│   │   └── vm_scale_sets.py
│   │
│   ├── 06_containers/
│   │   ├── create_aci.py
│   │   ├── setup_acr.py
│   │   ├── deploy_aks.py
│   │   └── kubernetes_operations.py
│   │
│   ├── 07_async/
│   │   ├── async_resource_creation.py
│   │   ├── parallel_operations.py
│   │   └── async_pagination.py
│   │
│   └── 08_advanced/
│       ├── error_handling.py
│       ├── retry_policies.py
│       ├── logging_practices.py
│       └── performance_optimization.py
│
├── notebooks/
│   ├── 01_sdk_basics.ipynb
│   ├── 02_authentication.ipynb
│   ├── 03_resource_management.ipynb
│   ├── 04_storage_operations.ipynb
│   └── 05_compute_resources.ipynb
│
├── scripts/
│   ├── setup_service_principal.sh     # Create service principal
│   ├── configure_rbac.sh              # Configure RBAC roles
│   └── cleanup_resources.sh           # Cleanup Azure resources
│
├── tests/
│   ├── __init__.py
│   ├── conftest.py
│   ├── test_authentication.py
│   ├── test_resource_groups.py
│   ├── test_storage.py
│   ├── test_network.py
│   └── test_compute.py
│
└── .github/
    └── workflows/
        ├── test.yml                   # Run tests
        └── examples.yml               # Test examples
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/vanHeemstraSystems/learning-idp-python-azure-sdk.git
cd learning-idp-python-azure-sdk
```

### 2. Set Up Python Environment

```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
# On Linux/MacOS:
source venv/bin/activate
# On Windows:
# venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
pip install -r requirements-dev.txt
```

### 3. Configure Azure Authentication

```bash
# Option 1: Azure CLI (recommended for development)
az login
az account set --subscription "your-subscription-id"

# Option 2: Service Principal
cp .env.example .env
# Edit .env with your credentials:
# AZURE_CLIENT_ID=your-client-id
# AZURE_CLIENT_SECRET=your-client-secret
# AZURE_TENANT_ID=your-tenant-id
# AZURE_SUBSCRIPTION_ID=your-subscription-id
```

### 4. Run Your First Example

```bash
# Test authentication
python examples/01_authentication/default_credential.py

# Create a resource group
python examples/02_resource_groups/create_resource_group.py
```

## 📖 Learning Path

Follow this recommended sequence:

### Week 1: SDK Fundamentals & Authentication

**Day 1-2: Understanding Azure SDK**

1. Read `docs/concepts/01-azure-sdk-overview.md`
1. Study `docs/concepts/02-authentication-patterns.md`
1. Run examples in `examples/01_authentication/`

**Day 3-4: Resource Management Basics**

1. Read `docs/guides/resource-management.md`
1. Complete `examples/02_resource_groups/`
1. Practice with `notebooks/03_resource_management.ipynb`

**Day 5-7: Core Services**

1. Work through storage examples (`examples/03_storage/`)
1. Explore networking examples (`examples/04_networking/`)
1. Complete exercises in notebooks

### Week 2: Advanced SDK Usage

**Day 1-3: Compute & Containers**

1. Study compute examples (`examples/05_compute/`)
1. Work with container examples (`examples/06_containers/`)
1. Build a complete infrastructure stack

**Day 4-5: Async Programming**

1. Read `docs/concepts/04-async-programming.md`
1. Complete `examples/07_async/`
1. Implement parallel resource creation

**Day 6-7: Best Practices & Optimization**

1. Study `docs/concepts/05-error-handling.md`
1. Review `docs/concepts/06-best-practices.md`
1. Complete `examples/08_advanced/`

### Week 3: Real-World Applications

**Day 1-3: Build Complete Solutions**

1. Infrastructure provisioning pipeline
1. Resource monitoring and management
1. Automated backup and recovery

**Day 4-5: Integration with IDP**

1. Service catalog implementation
1. Self-service portal backend
1. Automated compliance checking

**Day 6-7: Performance & Production**

1. Optimization techniques
1. Production-ready error handling
1. Logging and monitoring

## 🔑 Key Azure SDK Packages

### Core Packages

```python
# Authentication
azure-identity>=1.15.0              # Unified authentication

# Management (Control Plane)
azure-mgmt-resource>=23.0.0         # Resources, resource groups
azure-mgmt-subscription>=3.1.1      # Subscriptions
azure-mgmt-storage>=21.0.0          # Storage accounts
azure-mgmt-network>=25.0.0          # Networking
azure-mgmt-compute>=30.0.0          # VMs and compute
azure-mgmt-containerinstance>=10.1.0 # Container instances
azure-mgmt-containerservice>=28.0.0 # AKS
azure-mgmt-monitor>=6.0.0           # Monitoring

# Data Plane
azure-storage-blob>=12.19.0         # Blob storage
azure-storage-file-share>=12.15.0   # File shares
azure-keyvault-secrets>=4.7.0       # Key Vault secrets
```

## 💡 Authentication Examples

### DefaultAzureCredential (Recommended)

```python
from azure.identity import DefaultAzureCredential
from azure.mgmt.resource import ResourceManagementClient

# This tries multiple authentication methods in order:
# 1. Environment variables
# 2. Managed Identity
# 3. Azure CLI
# 4. Azure PowerShell
credential = DefaultAzureCredential()

# Use credential with any management client
resource_client = ResourceManagementClient(
    credential=credential,
    subscription_id="your-subscription-id"
)
```

### Service Principal Authentication

```python
from azure.identity import ClientSecretCredential
from azure.mgmt.resource import ResourceManagementClient

credential = ClientSecretCredential(
    tenant_id="your-tenant-id",
    client_id="your-client-id",
    client_secret="your-client-secret"
)

resource_client = ResourceManagementClient(
    credential=credential,
    subscription_id="your-subscription-id"
)
```

### Managed Identity (for Azure resources)

```python
from azure.identity import ManagedIdentityCredential
from azure.mgmt.resource import ResourceManagementClient

# System-assigned managed identity
credential = ManagedIdentityCredential()

# User-assigned managed identity
credential = ManagedIdentityCredential(
    client_id="your-managed-identity-client-id"
)

resource_client = ResourceManagementClient(
    credential=credential,
    subscription_id="your-subscription-id"
)
```

## 📝 Common Operations Examples

### Create Resource Group

```python
from azure.identity import DefaultAzureCredential
from azure.mgmt.resource import ResourceManagementClient

credential = DefaultAzureCredential()
resource_client = ResourceManagementClient(credential, subscription_id)

# Create resource group
resource_group_params = {
    'location': 'westeurope',
    'tags': {
        'environment': 'development',
        'project': 'idp-learning'
    }
}

resource_group = resource_client.resource_groups.create_or_update(
    'my-resource-group',
    resource_group_params
)

print(f"Created resource group: {resource_group.name}")
```

### Create Storage Account

```python
from azure.identity import DefaultAzureCredential
from azure.mgmt.storage import StorageManagementClient

credential = DefaultAzureCredential()
storage_client = StorageManagementClient(credential, subscription_id)

# Create storage account
storage_async_operation = storage_client.storage_accounts.begin_create(
    'my-resource-group',
    'mystorageaccount',
    {
        'sku': {'name': 'Standard_LRS'},
        'kind': 'StorageV2',
        'location': 'westeurope',
        'tags': {'purpose': 'learning'}
    }
)

storage_account = storage_async_operation.result()
print(f"Created storage account: {storage_account.name}")
```

### List Resources with Pagination

```python
from azure.identity import DefaultAzureCredential
from azure.mgmt.resource import ResourceManagementClient

credential = DefaultAzureCredential()
resource_client = ResourceManagementClient(credential, subscription_id)

# List all resource groups
for rg in resource_client.resource_groups.list():
    print(f"Resource Group: {rg.name}")
    print(f"  Location: {rg.location}")
    print(f"  Tags: {rg.tags}")
```

### Async Operations Example

```python
import asyncio
from azure.identity.aio import DefaultAzureCredential
from azure.mgmt.resource.resources.aio import ResourceManagementClient

async def create_multiple_resource_groups():
    credential = DefaultAzureCredential()
    async with ResourceManagementClient(credential, subscription_id) as client:
        # Create multiple resource groups in parallel
        tasks = []
        for i in range(5):
            rg_params = {'location': 'westeurope'}
            task = client.resource_groups.create_or_update(
                f'rg-{i}',
                rg_params
            )
            tasks.append(task)
        
        # Wait for all to complete
        results = await asyncio.gather(*tasks)
        return results

# Run async function
results = asyncio.run(create_multiple_resource_groups())
```

## 🎯 SDK Design Patterns

### 1. Client Initialization Pattern

```python
# Pattern: Initialize client once, reuse multiple times
class AzureResourceManager:
    def __init__(self, subscription_id: str):
        self.credential = DefaultAzureCredential()
        self.subscription_id = subscription_id
        self._resource_client = None
    
    @property
    def resource_client(self):
        if self._resource_client is None:
            self._resource_client = ResourceManagementClient(
                self.credential,
                self.subscription_id
            )
        return self._resource_client
```

### 2. Long-Running Operations Pattern

```python
# Many operations return a poller for long-running operations
from azure.core.polling import LROPoller

# Start operation (returns immediately)
poller: LROPoller = storage_client.storage_accounts.begin_create(...)

# Option 1: Wait for completion
result = poller.result()  # Blocks until complete

# Option 2: Check status
if not poller.done():
    print("Operation still running...")
    
# Option 3: Add callbacks
poller.add_done_callback(lambda p: print("Done!"))
```

### 3. Error Handling Pattern

```python
from azure.core.exceptions import (
    AzureError,
    ResourceNotFoundError,
    ResourceExistsError,
    HttpResponseError
)

try:
    resource_group = resource_client.resource_groups.get('my-rg')
except ResourceNotFoundError:
    print("Resource group not found")
    # Create it
    resource_client.resource_groups.create_or_update('my-rg', {...})
except HttpResponseError as e:
    print(f"HTTP error: {e.status_code} - {e.message}")
except AzureError as e:
    print(f"Azure SDK error: {e}")
```

### 4. Context Manager Pattern

```python
# Automatically close clients
from azure.identity import DefaultAzureCredential
from azure.mgmt.resource import ResourceManagementClient

credential = DefaultAzureCredential()

with ResourceManagementClient(credential, subscription_id) as client:
    # Use client
    for rg in client.resource_groups.list():
        print(rg.name)
# Client automatically closed
```

## 🔧 Development Tools

### Essential Tools

```bash
# Install development dependencies
pip install -r requirements-dev.txt

# Code formatting
black src/ examples/

# Linting
ruff check src/ examples/

# Type checking
mypy src/

# Run tests
pytest tests/
```

### Jupyter Notebooks

```bash
# Install Jupyter
pip install jupyter

# Start Jupyter
jupyter notebook notebooks/
```

## 📊 Performance Best Practices

### 1. Use Async for I/O Operations

```python
# Synchronous (slow)
for i in range(10):
    client.resource_groups.create_or_update(f'rg-{i}', {...})

# Asynchronous (fast)
import asyncio
from azure.mgmt.resource.resources.aio import ResourceManagementClient

async def create_rgs():
    async with ResourceManagementClient(...) as client:
        tasks = [
            client.resource_groups.create_or_update(f'rg-{i}', {...})
            for i in range(10)
        ]
        await asyncio.gather(*tasks)
```

### 2. Reuse Client Instances

```python
# Bad: Creating client for each operation
def get_resource_group(name):
    client = ResourceManagementClient(...)  # Expensive
    return client.resource_groups.get(name)

# Good: Reuse client
class ResourceManager:
    def __init__(self):
        self.client = ResourceManagementClient(...)
    
    def get_resource_group(self, name):
        return self.client.resource_groups.get(name)
```

### 3. Use Pagination Efficiently

```python
# Get only what you need
for page in resource_client.resources.list().by_page(page_size=100):
    for resource in page:
        process(resource)
        if should_stop():
            break
```

## 🔗 Related Repositories

- [learning-internal-development-platform](https://github.com/vanHeemstraSystems/learning-internal-development-platform) - Main overview
- [learning-idp-test-driven-development](https://github.com/vanHeemstraSystems/learning-idp-test-driven-development) - TDD with Azure SDK
- [learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code) - IaC patterns

## 🤝 Contributing

This is a personal learning repository, but suggestions and improvements are welcome!

1. Fork the repository
1. Create a feature branch
1. Make your changes
1. Ensure all tests pass
1. Submit a pull request

## 📄 License

This project is for educational purposes. See LICENSE file for details.

## 📧 Contact

Willem van Heemstra

- GitHub: [@vanHeemstraSystems](https://github.com/vanHeemstraSystems)
- LinkedIn: [Willem van Heemstra](https://www.linkedin.com/in/willemvanheemstra/)

-----

*Last updated: December 18, 2025*
*Part of the learning-internal-development-platform series*
