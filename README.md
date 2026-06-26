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
