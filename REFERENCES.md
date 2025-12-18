# References - Python Azure SDK for IDP

This document contains curated resources for learning the Azure SDK for Python to build and manage Internal Development Platforms (IDP).

## 📚 Table of Contents

- [Official Documentation](#official-documentation)
- [Books](#books)
- [Articles & Blog Posts](#articles--blog-posts)
- [Video Tutorials](#video-tutorials)
- [Online Courses](#online-courses)
- [Tools & Libraries](#tools--libraries)
- [GitHub Repositories](#github-repositories)
- [Related Learning Repositories](#related-learning-repositories)
- [Community Resources](#community-resources)

-----

## 📖 Official Documentation

### Azure SDK for Python

#### Core Documentation

- [Azure SDK for Python Documentation](https://learn.microsoft.com/en-us/azure/developer/python/) - Main documentation hub
- [Azure SDK for Python Design Guidelines](https://azure.github.io/azure-sdk/python_design.html) - Design principles
- [Azure SDK for Python GitHub](https://github.com/Azure/azure-sdk-for-python) - Source code repository
- [Azure SDK Releases](https://azure.github.io/azure-sdk/releases/latest/python.html) - Latest releases

#### Getting Started

- [Quickstart: Azure SDK for Python](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-overview) - Overview
- [Azure SDK for Python Setup](https://learn.microsoft.com/en-us/azure/developer/python/sdk/azure-sdk-install) - Installation guide
- [Configure Python for Azure](https://learn.microsoft.com/en-us/azure/developer/python/configure-local-development-environment) - Development setup

### Authentication & Identity

#### Azure Identity Library

- [azure-identity Documentation](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme) - Main docs
- [DefaultAzureCredential](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential) - Recommended credential
- [Authentication Patterns](https://learn.microsoft.com/en-us/azure/developer/python/sdk/authentication-overview) - Complete guide
- [Managed Identity](https://learn.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/overview) - Managed Identity overview

#### Service Principal

- [Create Service Principal](https://learn.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli) - Using Azure CLI
- [Service Principal Authentication](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme#service-principal-authentication) - SDK guide
- [RBAC for Service Principals](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview) - Role assignments

### Management Libraries

#### Resource Management

- [azure-mgmt-resource](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-resource-readme) - Resource operations
- [Resource Groups API](https://learn.microsoft.com/en-us/python/api/azure-mgmt-resource/azure.mgmt.resource.resources.v2022_09_01.operations.resourcegroupsoperations) - API reference
- [Resources API](https://learn.microsoft.com/en-us/python/api/azure-mgmt-resource/azure.mgmt.resource.resources.v2022_09_01.operations.resourcesoperations) - Resources operations

#### Storage Management

- [azure-mgmt-storage](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-storage-readme) - Storage management
- [azure-storage-blob](https://learn.microsoft.com/en-us/python/api/overview/azure/storage-blob-readme) - Blob operations
- [azure-storage-file-share](https://learn.microsoft.com/en-us/python/api/overview/azure/storage-file-share-readme) - File shares

#### Network Management

- [azure-mgmt-network](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-network-readme) - Network management
- [Virtual Networks](https://learn.microsoft.com/en-us/python/api/azure-mgmt-network/azure.mgmt.network.v2023_06_01.operations.virtualnetworksoperations) - VNet operations
- [Network Security Groups](https://learn.microsoft.com/en-us/python/api/azure-mgmt-network/azure.mgmt.network.v2023_06_01.operations.networksecuritygroupsoperations) - NSG operations

#### Compute Management

- [azure-mgmt-compute](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-compute-readme) - Compute management
- [Virtual Machines](https://learn.microsoft.com/en-us/python/api/azure-mgmt-compute/azure.mgmt.compute.v2023_07_01.operations.virtualmachinesoperations) - VM operations
- [Disks](https://learn.microsoft.com/en-us/python/api/azure-mgmt-compute/azure.mgmt.compute.v2023_04_02.operations.disksoperations) - Disk management

#### Container Services

- [azure-mgmt-containerinstance](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-containerinstance-readme) - Container Instances
- [azure-mgmt-containerservice](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-containerservice-readme) - AKS
- [azure-mgmt-containerregistry](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-containerregistry-readme) - Container Registry

#### Monitoring & Observability

- [azure-mgmt-monitor](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-monitor-readme) - Monitoring
- [Application Insights](https://learn.microsoft.com/en-us/azure/azure-monitor/app/api-custom-events-metrics) - App Insights API
- [Log Analytics](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/api/overview) - Log queries

### Core Functionality

#### Async Support

- [Async Client Library](https://learn.microsoft.com/en-us/python/api/overview/azure/core-readme#async-support) - Async patterns
- [AsyncIO with Azure SDK](https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/async.md) - Developer guide

#### Error Handling

- [azure.core.exceptions](https://learn.microsoft.com/en-us/python/api/azure-core/azure.core.exceptions) - Exception types
- [Error Handling Guide](https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/exceptions.md) - Best practices

#### Pagination

- [Pagination Support](https://learn.microsoft.com/en-us/python/api/overview/azure/core-readme#pagination) - Paging patterns
- [ItemPaged Class](https://learn.microsoft.com/en-us/python/api/azure-core/azure.core.paging.itempaged) - API reference

-----

## 📚 Books

### Azure Development

1. **“Azure for Architects”** by Ritesh Modi (3rd Edition)
- Azure architecture patterns
- Service design and implementation
- [Packt Publishing](https://www.packtpub.com/product/azure-for-architects-third-edition/9781803238562)
1. **“Python for DevOps”** by Noah Gift, Kennedy Behrman, Alfredo Deza, Grig Gheorghiu
- Python automation
- Cloud infrastructure with Python
- [O’Reilly](https://www.oreilly.com/library/view/python-for-devops/9781492057680/)
1. **“Practical Azure Application Development”** by Mitesh Soni
- Building applications on Azure
- Python SDK usage
- [Apress](https://link.springer.com/book/10.1007/978-1-4842-9254-3)

### Python Programming

1. **“Fluent Python”** by Luciano Ramalho (2nd Edition)
- Advanced Python patterns
- Async programming
- [O’Reilly](https://www.oreilly.com/library/view/fluent-python-2nd/9781492056348/)
1. **“Python Concurrency with asyncio”** by Matthew Fowler
- AsyncIO fundamentals
- Concurrent programming
- [Manning Publications](https://www.manning.com/books/python-concurrency-with-asyncio)

-----

## 📝 Articles & Blog Posts

### Azure SDK Fundamentals

#### Getting Started

- [Azure SDK for Python: A Comprehensive Guide](https://devblogs.microsoft.com/azure-sdk/azure-sdk-for-python-comprehensive-guide/) - Microsoft
- [Working with Azure Python SDK](https://azure.github.io/azure-sdk/releases/latest/python.html) - Azure SDK Team
- [Azure SDK Design Guidelines Explained](https://devblogs.microsoft.com/azure-sdk/azure-sdk-design-guidelines-explained/) - Microsoft DevBlog

#### Authentication Deep Dives

- [Understanding DefaultAzureCredential](https://devblogs.microsoft.com/azure-sdk/authentication-and-the-azure-sdk/) - Microsoft
- [Managed Identity Best Practices](https://techcommunity.microsoft.com/t5/azure-developer-community-blog/managed-identity-best-practices/ba-p/3678841) - Azure Community
- [Service Principal Authentication Patterns](https://docs.microsoft.com/en-us/azure/developer/python/azure-sdk-authenticate) - Microsoft Docs

### Performance & Optimization

- [Optimizing Azure SDK Performance](https://devblogs.microsoft.com/azure-sdk/performance-improvements-in-the-new-azure-sdks/) - Azure SDK Blog
- [Async Patterns with Azure SDK](https://devblogs.microsoft.com/azure-sdk/async-support-in-the-azure-sdk-for-python/) - Microsoft
- [Connection Pooling and Retries](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#http-pipeline) - GitHub Docs

### Best Practices

- [Azure SDK Best Practices](https://azure.github.io/azure-sdk/python_introduction.html) - Official guide
- [Error Handling in Azure SDK](https://devblogs.microsoft.com/azure-sdk/improved-error-handling-in-azure-sdk/) - Microsoft
- [Logging and Diagnostics](https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/logging.md) - GitHub guide

### Real-World Scenarios

- [Building an IDP with Azure SDK](https://techcommunity.microsoft.com/t5/azure-developer-community-blog/building-internal-developer-platforms-on-azure/ba-p/3894567) - Azure Community
- [Infrastructure Automation with Python](https://cloudskills.io/blog/azure-automation-python) - Cloud Skills
- [Azure Resource Management at Scale](https://techcommunity.microsoft.com/t5/azure-architecture-blog/managing-azure-at-scale/ba-p/3289476) - Azure Architecture

-----

## 🎥 Video Tutorials

### Official Microsoft Content

#### Azure SDK Tutorials

- [Azure SDK for Python Overview](https://learn.microsoft.com/en-us/shows/azure-friday/azure-sdk-for-python-overview) - Azure Friday (30 min)
- [Getting Started with Azure SDK](https://learn.microsoft.com/en-us/shows/azure-enablement/getting-started-with-azure-sdk-for-python) - Azure Enablement (45 min)
- [Authentication with Azure Identity](https://www.youtube.com/watch?v=F6vJwxgaeO8) - Microsoft (20 min)

#### Deep Dives

- [Azure SDK Architecture](https://mybuild.microsoft.com/sessions/azure-sdk-for-python-deep-dive) - Microsoft Build (60 min)
- [Async Programming with Azure SDK](https://channel9.msdn.com/Shows/On-NET/Async-programming-with-Azure-SDK) - Channel 9 (25 min)
- [Best Practices for Production](https://www.youtube.com/watch?v=mXF2hGgqfMU) - Azure (40 min)

### Community Content

#### Conference Talks

- [Python on Azure](https://www.youtube.com/watch?v=Rt3rLvj59ZU) - PyCon (45 min)
- [Building Cloud-Native Apps](https://www.youtube.com/watch?v=h9G2j2ktMVA) - EuroPython (50 min)
- [Infrastructure as Code with Python](https://www.youtube.com/watch?v=XdXG8-cP5kU) - PyCascades (30 min)

#### Tutorial Series

- [Azure Python SDK Tutorial Series](https://www.youtube.com/playlist?list=PLLasX02E8BPBxGouWlJV-u-XZWOc2RkiX) - Microsoft DevRadio
- [Python for Azure Developers](https://www.youtube.com/playlist?list=PLXtHYVsvn_b-cxvz_K_p-nJ0vSrgZe_MZ) - Cloud Academy

-----

## 🎓 Online Courses

### Microsoft Learn (Free)

#### Learning Paths

- [Azure for Python Developers](https://learn.microsoft.com/en-us/training/paths/python-azure/) - Complete path
- [Introduction to Azure SDK for Python](https://learn.microsoft.com/en-us/training/modules/intro-to-azure-python/) - Module
- [Authenticate Python apps to Azure services](https://learn.microsoft.com/en-us/training/modules/python-authentication-azure-services/) - Module
- [Build serverless apps with Python](https://learn.microsoft.com/en-us/training/paths/build-python-serverless-apps-azure/) - Learning path

#### Certifications

- [AZ-204: Developing Solutions for Microsoft Azure](https://learn.microsoft.com/en-us/certifications/azure-developer/) - Certification
- [AZ-305: Designing Azure Infrastructure Solutions](https://learn.microsoft.com/en-us/certifications/azure-solutions-architect/) - Certification

### Paid Platforms

#### Pluralsight

- [Azure for Python Developers](https://www.pluralsight.com/paths/azure-for-python-developers) - Learning path
- [Developing with Azure SDK](https://www.pluralsight.com/courses/developing-azure-sdk) - Course
- [Python Async Programming](https://www.pluralsight.com/courses/python-async-programming) - Course

#### LinkedIn Learning

- [Python on Azure](https://www.linkedin.com/learning/paths/python-on-azure) - Learning path
- [Azure SDK for Developers](https://www.linkedin.com/learning/azure-sdk-for-developers) - Course

#### Udemy

- [Azure Python Development](https://www.udemy.com/course/azure-python-development/) - Course
- [Master Azure SDK for Python](https://www.udemy.com/course/master-azure-sdk-python/) - Course

-----

## 🛠️ Tools & Libraries

### Core Azure SDK Packages

#### Identity & Authentication

- **[azure-identity](https://pypi.org/project/azure-identity/)** - Unified authentication
  - `DefaultAzureCredential` - Auto credential chain
  - `ClientSecretCredential` - Service principal
  - `ManagedIdentityCredential` - Managed identity
  - `AzureCliCredential` - Azure CLI auth

#### Management Libraries

- **[azure-mgmt-resource](https://pypi.org/project/azure-mgmt-resource/)** - Resource management
- **[azure-mgmt-storage](https://pypi.org/project/azure-mgmt-storage/)** - Storage management
- **[azure-mgmt-network](https://pypi.org/project/azure-mgmt-network/)** - Network management
- **[azure-mgmt-compute](https://pypi.org/project/azure-mgmt-compute/)** - Compute management
- **[azure-mgmt-containerinstance](https://pypi.org/project/azure-mgmt-containerinstance/)** - Container instances
- **[azure-mgmt-containerservice](https://pypi.org/project/azure-mgmt-containerservice/)** - AKS
- **[azure-mgmt-monitor](https://pypi.org/project/azure-mgmt-monitor/)** - Monitoring

#### Data Plane Libraries

- **[azure-storage-blob](https://pypi.org/project/azure-storage-blob/)** - Blob storage
- **[azure-storage-file-share](https://pypi.org/project/azure-storage-file-share/)** - File shares
- **[azure-keyvault-secrets](https://pypi.org/project/azure-keyvault-secrets/)** - Key Vault secrets
- **[azure-keyvault-keys](https://pypi.org/project/azure-keyvault-keys/)** - Key Vault keys

#### Core Libraries

- **[azure-core](https://pypi.org/project/azure-core/)** - Core functionality
  - Async support
  - Pagination
  - Polling
  - Exceptions

### Development Tools

#### Code Quality

- **[black](https://black.readthedocs.io/)** - Code formatting
- **[ruff](https://docs.astral.sh/ruff/)** - Fast linting
- **[mypy](http://mypy-lang.org/)** - Type checking
- **[pylint](https://pylint.org/)** - Code analysis

#### Testing

- **[pytest](https://pytest.org/)** - Testing framework
- **[pytest-asyncio](https://pytest-asyncio.readthedocs.io/)** - Async testing
- **[pytest-mock](https://pytest-mock.readthedocs.io/)** - Mocking
- **[responses](https://github.com/getsentry/responses)** - Mock HTTP

#### Documentation

- **[sphinx](https://www.sphinx-doc.org/)** - Documentation generator
- **[pdoc](https://pdoc.dev/)** - API documentation
- **[mkdocs](https://www.mkdocs.org/)** - Project documentation

#### Utilities

- **[python-dotenv](https://pypi.org/project/python-dotenv/)** - Environment variables
- **[pydantic](https://docs.pydantic.dev/)** - Data validation
- **[tenacity](https://tenacity.readthedocs.io/)** - Retry logic
- **[structlog](https://www.structlog.org/)** - Structured logging

### Azure CLI & Tools

- **[Azure CLI](https://learn.microsoft.com/en-us/cli/azure/)** - Command-line tool
- **[Azure PowerShell](https://learn.microsoft.com/en-us/powershell/azure/)** - PowerShell module
- **[Azure Storage Explorer](https://azure.microsoft.com/en-us/products/storage/storage-explorer/)** - GUI for storage
- **[Azure Data Studio](https://azure.microsoft.com/en-us/products/data-studio/)** - Database tool

-----

## 💻 GitHub Repositories

### Official Microsoft Repositories

#### Azure SDK

- [Azure SDK for Python](https://github.com/Azure/azure-sdk-for-python) - Main repository
- [Azure SDK Design Guidelines](https://github.com/Azure/azure-sdk) - Cross-language guidelines
- [Azure SDK Tools](https://github.com/Azure/azure-sdk-tools) - Development tools

#### Sample Code

- [Azure Samples - Python](https://github.com/Azure-Samples/azure-samples-python-management) - Management samples
- [Azure Python Labs](https://github.com/Azure-Samples/azure-python-labs) - Hands-on labs
- [Azure Functions Python Samples](https://github.com/Azure-Samples/azure-functions-python-samples) - Functions examples

#### Templates & Starter Kits

- [Azure Python Developer Resources](https://github.com/Azure-Samples/python-docs-hello-world) - Getting started
- [Azure DevOps Python Samples](https://github.com/microsoft/azure-devops-python-samples) - DevOps examples

### Community Repositories

#### Learning Resources

- [Awesome Azure](https://github.com/kristofferandreasen/awesome-azure) - Curated Azure resources
- [Azure SDK Samples](https://github.com/Azure-Samples) - Official samples organization
- [Python Azure Examples](https://github.com/realpython/python-azure-examples) - Real Python examples

#### Tools & Utilities

- [Azure CLI Extensions](https://github.com/Azure/azure-cli-extensions) - CLI extensions
- [Azure DevOps Python API](https://github.com/microsoft/azure-devops-python-api) - DevOps SDK
- [Azure Functions Python Worker](https://github.com/Azure/azure-functions-python-worker) - Functions runtime

-----

## 🔗 Related Learning Repositories

### From learning-internal-development-platform Series

1. **[learning-internal-development-platform](https://github.com/vanHeemstraSystems/learning-internal-development-platform)**
- Main overview repository
- Complete learning roadmap
- Architecture patterns
1. **[learning-idp-test-driven-development](https://github.com/vanHeemstraSystems/learning-idp-test-driven-development)**
- TDD practices for Azure SDK
- Unit and integration testing
- Mocking Azure services
1. **[learning-idp-platform-engineering](https://github.com/vanHeemstraSystems/learning-idp-platform-engineering)**
- Platform engineering concepts
- IDP architecture
- Service catalogs
1. **[learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code)**
- Bicep and ARM templates
- Terraform on Azure
- IaC best practices
1. **[learning-idp-azure-compute](https://github.com/vanHeemstraSystems/learning-idp-azure-compute)**
- VM management with SDK
- Container orchestration
- Compute optimization
1. **[learning-idp-azure-networking](https://github.com/vanHeemstraSystems/learning-idp-azure-networking)**
- Network topology with SDK
- Security groups
- Load balancing
1. **[learning-idp-azure-storage](https://github.com/vanHeemstraSystems/learning-idp-azure-storage)**
- Storage account management
- Blob and file operations
- Data lifecycle
1. **[learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines)**
- Azure Pipelines
- GitHub Actions
- Automated deployments

-----

## 👥 Community Resources

### Forums & Discussion

#### Official Microsoft

- [Microsoft Q&A - Azure SDK](https://learn.microsoft.com/en-us/answers/tags/158/azure-sdk) - Official Q&A
- [Azure SDK GitHub Discussions](https://github.com/Azure/azure-sdk-for-python/discussions) - SDK discussions
- [Azure Tech Community](https://techcommunity.microsoft.com/t5/azure-developer-community-blog/bg-p/AzureDevCommunityBlog) - Developer blog

#### Stack Overflow

- [azure-sdk-python](https://stackoverflow.com/questions/tagged/azure-sdk-python) - SDK questions
- [azure-python](https://stackoverflow.com/questions/tagged/azure-python) - Azure Python
- [azure](https://stackoverflow.com/questions/tagged/azure) - General Azure

### Social Media & Communities

#### Discord & Slack

- [Azure Community Discord](https://discord.gg/azure) - Community chat
- [Python Discord](https://discord.gg/python) - Python community
- [Cloud Native Computing Foundation Slack](https://slack.cncf.io/) - CNCF community

#### Reddit

- [r/Azure](https://www.reddit.com/r/AZURE/) - Azure discussions
- [r/Python](https://www.reddit.com/r/Python/) - Python community
- [r/devops](https://www.reddit.com/r/devops/) - DevOps practices

### Blogs & Newsletters

#### Microsoft Blogs

- [Azure SDK Blog](https://devblogs.microsoft.com/azure-sdk/) - Official SDK blog
- [Python @ Microsoft](https://devblogs.microsoft.com/python/) - Python at Microsoft
- [Azure Developer Community Blog](https://techcommunity.microsoft.com/t5/azure-developer-community-blog/bg-p/AzureDevCommunityBlog) - Community content

#### Community Blogs

- [Real Python - Azure](https://realpython.com/tutorials/azure/) - Python Azure tutorials
- [TestDriven.io](https://testdriven.io/blog/) - Testing and DevOps
- [Cloud Skills](https://cloudskills.io/blog) - Cloud development

-----

## 📊 Cheat Sheets & Quick References

### Azure SDK Quick References

- [Azure SDK for Python Cheat Sheet](https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/cheat_sheet.md) - Quick reference
- [Authentication Cheat Sheet](https://learn.microsoft.com/en-us/azure/developer/python/sdk/authentication-overview#authentication-decision-tree) - Auth patterns
- [Common Operations Guide](https://learn.microsoft.com/en-us/azure/developer/python/sdk/examples) - Code examples

### Python Quick References

- [Python AsyncIO Cheat Sheet](https://www.pythonsheets.com/notes/python-asyncio.html) - Async patterns
- [Python Type Hints](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html) - Type annotations

### Azure CLI

- [Azure CLI Reference](https://learn.microsoft.com/en-us/cli/azure/reference-index) - Command reference
- [Azure CLI Tips and Tricks](https://learn.microsoft.com/en-us/cli/azure/use-cli-effectively) - Best practices

-----

## 🎯 Next Steps

After mastering Python Azure SDK, continue with:

1. **[learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code)** - IaC patterns
1. **[learning-idp-azure-compute](https://github.com/vanHeemstraSystems/learning-idp-azure-compute)** - Compute resources
1. **[learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines)** - CI/CD automation
1. **[learning-idp-observability](https://github.com/vanHeemstraSystems/learning-idp-observability)** - Monitoring and logging

-----

*Last updated: December 18, 2025*
*Part of the learning-internal-development-platform series*
