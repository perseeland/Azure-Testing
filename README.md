# Azure Testing Dashboard

A comprehensive security testing and reconnaissance guide for Azure (Entra ID) environments. This project contains interactive HTML dashboards and detailed documentation for Azure security assessment, penetration testing, and cloud infrastructure reconnaissance.

## 📁 Project Structure

```
Azure Testing/
├── Tools & Authentication
│   ├── az-cli.html              # Azure CLI authentication and usage
│   ├── az-powershell.html       # Azure PowerShell guide with object inspection
│   ├── tokens.html              # Token acquisition and manipulation
│   ├── roadtx.html              # ROADtools token exchange guide
│   ├── aadinternals.html        # AADInternals PowerShell module guide
│   ├── graphrunner.html         # GraphRunner tool documentation
│   └── cloud-prowl.html         # Cloud reconnaissance tool guide
│
├── Attack Scenarios & Exploitation
│   ├── cap.html                 # Conditional Access Bypass techniques
│   ├── mfa.html                 # MFA bypass and validation techniques
│   ├── phs.html                 # Password Hash Sync exploitation
│   ├── managed-identity.html    # Managed Identity exploitation
│   └── power-platform.html      # Power Platform/Business Apps security
│
├── Reconnaissance & Enumeration
│   ├── external-recon.html      # External Azure reconnaissance
│   ├── internal-recon.html      # Internal Azure resource enumeration
│   ├── identity-users-creds.html # User enumeration and credential validation
│   └── mg-graph.html            # Microsoft Graph API queries
│
├── Azure Resources
│   ├── storage-account.html     # Azure Storage account exploitation
│   ├── container-app.html       # Container App security testing
│   ├── virtual-machines.html    # VM enumeration and exploitation
│   ├── automation-account.html  # Automation Account privilege escalation
│   ├── automation.html          # Azure Automation runbook exploitation
│   ├── azure-key-vault.html     # Key Vault secret extraction
│   ├── mysql-flexible-server.html # MySQL database server testing
│   ├── network.html             # Network security group enumeration
│   └── sites.html               # Web App/App Service testing
│
├── Utilities
│   ├── azure.css                # Styling and UI components
│   └── azure.js                 # JavaScript utilities for interactive tools
```

## 🎯 Key Features

### Interactive Dashboards
Each HTML file provides an interactive dashboard with:
- **Input fields** for credentials, tokens, and parameters
- **Copy-to-clipboard buttons** for easy command execution
- **Multi-language support** (bash, PowerShell, CLI commands)
- **Dynamic command generation** based on user inputs
- **Local storage** to save frequently used values

### Comprehensive Coverage

#### Authentication & Token Acquisition
- Multiple authentication methods (ROPC, device code, interactive)
- Token exchange and manipulation
- Refresh token usage
- Multi-factor authentication bypass techniques
- Service principal authentication

#### Azure AD / Entra ID Reconnaissance
- User enumeration techniques
- Group membership discovery
- Tenant information gathering
- Service principal identification
- Application and permission mapping

#### Resource Exploitation
- Storage account enumeration and access
- Container analysis
- Virtual machine discovery and management
- Key vault secret extraction
- Automation account runbook access
- Database server enumeration

#### Advanced Techniques
- Conditional Access Policy bypass
- MFA bypass and validation attacks
- Password Hash Sync exploitation
- Managed Identity abuse
- Power Platform exploitation
- Cross-tenant resource access

## 🔧 Tool Reference

### Microsoft Graph API
- REST API calls for querying directory objects
- User, group, and application enumeration
- Mail and OneDrive access
- Device compliance queries

### ROADtools (roadtx)
- Token exchange across Microsoft services
- Refresh token manipulation
- FOCI (Families of Client IDs) support
- Multi-resource token acquisition

### AADInternals
- PowerShell module for Azure AD enumeration
- Token acquisition and analysis
- Domain controller enumeration
- Privileged user identification

### Cloud Reconnaissance Tools
- Azure resource discovery
- Tenant mapping
- Cross-tenant enumeration
- Public IP identification

## 📊 Typical Workflow

1. **Reconnaissance Phase**
   - Use `external-recon.html` for initial tenant discovery
   - Enumerate users with `identity-users-creds.html`
   - Map resources with `internal-recon.html`

2. **Authentication Phase**
   - Attempt credential validation
   - Acquire tokens using `tokens.html`
   - Explore token-based access

3. **Exploitation Phase**
   - Test conditional access with `cap.html`
   - Attempt MFA bypass with `mfa.html`
   - Exploit specific services (storage, Key Vault, etc.)

4. **Privilege Escalation**
   - Leverage managed identities
   - Exploit automation accounts
   - Access sensitive resources

## ⚠️ Disclaimer

**This toolkit is for authorized security testing and educational purposes only.**

- Only use these tools in environments you own or have explicit permission to test
- Unauthorized access to computer systems is illegal
- Ensure compliance with local laws and regulations
- Obtain written authorization before conducting security assessments
- Responsible disclosure of vulnerabilities is required

## 🔐 Security Considerations

All credentials and sensitive values in this dashboard are **placeholder examples**:
- Email addresses are anonymized
- Passwords are replaced with generic placeholders
- Tenant IDs and object IDs are sanitized
- Token snippets are truncated/redacted
- No real credentials are included

Replace placeholders with actual values during testing.

## 📚 Tools & Frameworks Used

- **Microsoft Graph API** - Directory and resource queries
- **Azure CLI** - Command-line Azure management
- **Azure PowerShell** - PowerShell Azure management
- **ROADtools** - Azure token manipulation
- **AADInternals** - Azure AD reconnaissance
- **GraphRunner** - Automated Graph API exploitation
- **Cloud Prowl** - Azure cloud reconnaissance

## 🚀 Getting Started

1. Navigate to the `Azure Testing/` folder
2. Open any HTML file in a web browser based on your testing phase:
   - Start with `external-recon.html` for initial reconnaissance
   - Use `tokens.html` for token acquisition
   - Choose specific tools for exploitation
3. Follow the step-by-step instructions in each guide
4. Use the interactive input fields to customize commands
5. Copy commands and execute them in your terminal

## 📝 File Details

| File | Purpose | Type |
|------|---------|------|
| `tokens.html` | Token acquisition and exchange | Guide |
| `cap.html` | Conditional Access Bypass | Exploitation |
| `mfa.html` | MFA validation and bypass | Exploitation |
| `managed-identity.html` | Managed Identity exploitation | Exploitation |
| `storage-account.html` | Storage account enumeration | Reconnaissance |
| `identity-users-creds.html` | User and credential validation | Reconnaissance |
| `roadtx.html` | ROADtools token exchange | Tool Guide |
| `mg-graph.html` | Microsoft Graph API queries | Tool Guide |
| `phs.html` | Password Hash Sync exploitation | Exploitation |
| `internal-recon.html` | Resource enumeration | Reconnaissance |
| `external-recon.html` | External tenant discovery | Reconnaissance |

## 💡 Tips for Effective Use

1. **Start with reconnaissance** - Understand the target environment first
2. **Document findings** - Keep track of discovered resources and permissions
3. **Test systematically** - Follow a structured approach to avoid missing vectors
4. **Verify assumptions** - Confirm access and permissions before exploitation
5. **Take screenshots** - Document your testing process for reports

## 🔄 Updates & Improvements

This dashboard is continuously updated with:
- New Azure security features
- Emerging attack techniques
- Tool updates and improvements
- Community-suggested additions

## 📧 Contact & Attribution

- **Author**: Security Testing Dashboard
- **Purpose**: Educational and authorized security testing
- **License**: For authorized use only

---

**Last Updated**: June 27, 2026

For questions or contributions, please refer to the project repository.
