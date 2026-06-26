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
