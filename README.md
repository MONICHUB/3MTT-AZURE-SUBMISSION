# 1. Azure Account Setup & Registration Journey

To establish a secure, isolated sandbox environment for cloud deployment, a formal onboarding sequence must be executed. Because an active environment has already been successfully provisioned, this section retroactively maps the complete registration journey and verification milestones required to activate an administrative tenant.

### Step-by-Step Enrollment Sequence

1. **Initiate the Portal Gateway:**
Navigate to the official Microsoft Azure portal (`https://azure.microsoft.com`). Select the prominent **"Start free"** call-to-action button to redirect the browser to the Microsoft identity enrollment subsystem.

2. **Microsoft Identity Creation:**
Log in using an existing, verified personal Microsoft account (Outlook/Hotmail). If an account does not exist, initialize the creation of a new administrative identity profile (e.g., `yourname@outlook.com`).

3. **Personal Profile & Contact Validation:**
Input formal account registration details, including your full legal name, region, and a valid email address. The system automatically sends an alphanumeric verification token to the designated email account. You must copy and input this token to progress past the email validation gate.

4. **Two-Factor Phone Authentication:**
Provide a valid mobile phone number for text or voice verification. Select **"Send text message"** or **"Call me"** to receive a one-time password (OTP). Input the code into the verification interface within the expiration window to confirm active identity ownership.

5. **Financial Identity Verification (Credit Card Validation):**
Submit valid credit card information (cardholder name, card number, expiration, and CVV).
* *Critical Compliance Note:* Microsoft strictly enforces this step to validate identity and mitigate automated bot registration. While a temporary $1 authorization hold may briefly appear to verify card validity, **no charges will be applied** to the payment method during the lifespan of the Free Tier.

6. **Agreement & Tenant Provisioning:**
Review and accept the Microsoft Customer Agreement and the privacy statement checkboxes. Click **"Sign up"** to trigger the background automated infrastructure provisioning. The system redirects the session to the initialized Azure Portal dashboard under an active subscription state.

---

### Verification and Subscription Status

To verify that the account was correctly created and that the subscription is structurally active without errors, navigate to the portal's global search bar and look up "Subscriptions". The workspace should display an active sandbox environment matching the target verification image below.

![Active Azure Subscription](azure subscription 1.png)


1 of 204
(no subject)
Inbox

ogboji monica <ogbojimonic@gmail.com>
4:22 PM (0 minutes ago)
to me




# 2. Azure Free Tier Limits & Benefits Summary

To maintain effective cost control and maximize efficiency, this deployment utilizes the structured guidelines of the Azure Free Tier. The subscription is bound by the following baseline parameters:

### Core Account Benefits
* **$200 Free Credit:** A complementary credit allocated for the first 30 days of service activation. This credit applies across all Azure workloads to allow sandbox testing without out-of-pocket costs.
* **12 Months of Popular Free Services:** Extended, metered access to a specific suite of popular products for a full year post-activation (such as limited virtual compute hours and storage options).
* **Always Free Services:** Unrestricted, continuous access to over 55+ baseline services within standard monthly consumption thresholds.

### Standard Resource Quota Matrix
To remain within the strict free boundaries and avoid premature credit exhaustion, infrastructure provisioning targets the following free resource tier thresholds:

| Service Category | Free Tier Allocation Limit | Operational Guardrails |
| :--- | :--- | :--- |
| **Linux Virtual Machines** | 750 Hours / Month | Must utilize `B1s` burstable compute shapes |
| **Windows Virtual Machines** | 750 Hours / Month | Must utilize `B1s` burstable compute shapes |
| **Azure Blob Storage** | 5 GB of LRS Storage | Capped at 20,000 Read & 10,000 Write operations |
| **Azure SQL Database** | 250 GB storage capacity | Strictly limited to standard `S0` database 



# 3. Azure Portal Navigation & Dashboard Customization

To manipulate resources effectively within an enterprise cloud infrastructure, administrators must master the primary structural control planes of the Azure Management Portal.

### Core Interface Mechanics

* **Global Search Bar:** Located at the top center of the user interface. This is the primary command tool used to rapidly locate services, specific resource names, documentation, or active deployment tenants without digging through multi-nested menus.
* **Portal Sidebar Menu:** Accessible via the hamburger navigation icon on the top-left corner. It pins essential service shortcut locations—such as *All Resources*, *Resource Groups*, *App Services*, and *Virtual Machines*—for swift horizontal navigation.
* **Azure Marketplace Gateway:** Found via the main menu or global search. It acts as an integrated catalog enabling deployment of pre-configured third-party or native solutions directly into the tenant scope.

### Custom Dashboard Implementation
To optimize monitoring workflows and demonstrate configuration capabilities, a personalized monitoring dashboard layout was instantiated within the root directory portal directory. By entering portal modification mode, the default landing profile was re-architected to display customized layout elements, real-time platform metrics, and critical service health matrices.

![Customized Azure Portal Dashboard Architecture](custom_dashboard.png)


# 4. Identity, Governance, and Security Configurations

Cloud security is managed under the **Shared Responsibility Model**. While Microsoft assumes structural responsibility for securing physical data centers, host hypervisors, and core networking layers, the tenant administrator retains absolute responsibility for securing data assets, operational endpoints, and user identities.

### Multi-Factor Authentication (MFA) Implementation Guide
To mitigate identity compromises and protect root administrative privileges from credential theft, Multi-Factor Authentication must be enforced across the tenant using Microsoft Entra ID Security Defaults:

1. Navigate to the global search bar at the top of the portal, search for **Microsoft Entra ID**, and click on the service directory.
2. In the upper horizontal menu navigation pane, select the **Properties** tab.
3. Scroll down to the **Security defaults** sub-section.
4. Verify or select the **Manage security defaults** hyperlink interface to ensure security configurations are active. This status structurally enforces modern MFA challenges across all users and administrative accounts within the cloud directory tenant to protect against credential threats.

![Microsoft Entra ID Governance and MFA Security Configuration](mfa_security_defaults.png)

### Governance Frameworks & Password Policies
Beyond baseline MFA activation, the environment is hardened through two structural administrative layers:

* **Role-Based Access Control (RBAC):** Implemented via the **Access Control (IAM)** blade embedded within resources and resource groups. Permissions are governed strictly by the **Principle of Least Privilege (PoLP)**, ensuring that identities are provisioned with only the absolute minimum required permissions necessary to complete their functions, rather than default global admin permissions.
* **Tenant Password Policies:** Managed through the authentication methods and user settings within Entra ID. The environment enforces strong complex structures (requiring alphanumeric combinations, special characters, and minimum character counts) while structurally logging all sign-in behaviors via the Audit Logs stream for continuous security visibility.

Billing Alerts & Cost Management Architectures

Deploying enterprise infrastructure inside a public cloud framework demands strict financial governance. Under the consumption-based pricing model of cloud computing, unmonitored resources can scale dynamically, leading to unexpected fiscal overhead or complete credit depletion.

### Automated Budget & Consumption Guardrails
To prevent accidental over-expenditure and ensure continuous compliance with the Azure Free Tier boundaries, an active automated financial control budget has been established within the **Cost Management + Billing** workspace:

1. **Budget Threshold Definition:** An operational baseline budget profile (`project101_budget`) has been instantiated to monitor real-time monthly cumulative expenditures.
2. **Dynamic Alert Conditions:** Automated notification parameters trigger when consumption vectors cross or project toward critical percentage thresholds of the assigned budget.
3. **Notification Routing Protocols:** The budget subsystem bridges directly with automated communications, routing event flags to the administrator's structural email endpoint (`ogbojimonic@gmail.com`) to allow for rapid optimization, manual scaling holds, or asset evaluation prior to generating overages.

![Cost Management )







