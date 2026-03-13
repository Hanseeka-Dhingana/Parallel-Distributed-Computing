# Practice Problems on Cloud SLA & Availability

## 1. Basic SLA Violation

A cloud provider guarantees **99% availability**.
An application runs **12 hours per day**.

After **30 days**, the total downtime is **11 hours**.

**Question:**
Did the provider violate the SLA?

---

# 2. Allowed Downtime Calculation

A provider guarantees **99.9% availability** for a service running **24 hours per day**.

**Question:**
Calculate the **maximum downtime allowed in 30 days**.

---

# 3. Availability Percentage Calculation

A system runs **24 hours per day** for **30 days**.
During this period, the service was unavailable for **5 hours**.

**Question:**
Calculate the **actual availability percentage**.

---

# 4. Daily Usage Scenario

A cloud service promises **99% availability**.
A company uses the service **10 hours per day**.

At the end of **30 days**, the outage recorded is **4 hours**.

**Question:**
Check whether the SLA was violated.

---

# 5. Weekly Availability

A cloud provider promises **98% availability**.

An application runs **24 hours daily** for **7 days**.

Total downtime recorded is **6 hours**.

**Question:**
Calculate the availability and determine whether SLA is satisfied.

---

# 6. Allowed Downtime Per Day

A provider offers **99.5% availability**.

**Question:**
What is the **maximum downtime allowed per day** if the service runs **24 hours daily**?

---

# 7. Finding Downtime From Availability

A system guarantees **99% availability**.

Total time in a month = **720 hours**.

**Question:**
What is the **maximum downtime allowed**?

---

# 8. Real Availability vs SLA

A cloud provider guarantees **99.8% availability**.

During **30 days (720 hours)**, the total downtime recorded is **3 hours**.

**Question:**
Calculate the **actual availability** and check if SLA is met.

---

# 9. Multiple Outages

A cloud service promises **99% availability**.

Service runs **24 hours per day for 30 days**.

Outages occurred:

* 2 hours
* 3 hours
* 4 hours
* 1 hour

**Question:**
Calculate total downtime and determine SLA violation.

---

# 10. Application Runs Limited Hours

A cloud provider guarantees **99% availability**.

An application runs only **8 hours per day**.

After **30 days**, the total downtime is **3 hours**.

**Question:**
Check whether the SLA was violated.

---

# 11. Comparing Two Providers

Two cloud providers offer services:

Provider A → **99% availability**
Provider B → **99.9% availability**

**Question:**
Calculate the **maximum downtime allowed in a month (720 hours)** for both providers.

---

# 12. Yearly SLA

A provider guarantees **99% availability for a year**.

Total hours in a year = **8760 hours**

**Question:**
What is the **maximum downtime allowed per year**?

---

# 13. Real System Availability

A cloud service ran **720 hours in a month**.

Downtime recorded = **15 hours**

**Question:**
Calculate the **availability percentage**.

---

# 14. SLA Guarantee Check

A cloud provider promises **99.5% availability**.

An application runs **12 hours per day** for **30 days**.

Total downtime = **2 hours**.

**Question:**
Check whether SLA guarantee is violated.

---

# 15. Maximum Downtime for 99.99%

A critical banking system requires **99.99% availability**.

Total monthly runtime = **720 hours**.

**Question:**
Calculate the **maximum downtime allowed**.

---

# 16. Real Availability Calculation

A cloud system runs **720 hours per month**.

Downtime = **10 hours**.

**Question:**
Calculate the **availability percentage**.

---

# 17. SLA Check with High Availability

A provider guarantees **99.9% availability**.

Total runtime = **720 hours**

Downtime recorded = **1.5 hours**.

**Question:**
Did the provider violate the SLA?

---

# 18. Maximum Allowed Downtime for 98%

A cloud provider offers **98% availability**.

Total runtime = **720 hours per month**.

**Question:**
Calculate the maximum downtime allowed.

---

# 19. Real Availability vs Required

A service requires **99% availability**.

Total runtime = **720 hours**

Downtime recorded = **8 hours**.

**Question:**
Calculate availability and check SLA compliance.

---

# 20. Application Specific SLA

A cloud provider guarantees **99% availability**.

An application runs **6 hours per day for 30 days**.

Total downtime = **2 hours**.

**Question:**
Determine if the SLA guarantee is violated.

---
# Practice SLA Scenario Questions


# 1️⃣ Cloud SLA Case

A company signs an SLA with a cloud provider guaranteeing **99% availability** for a **30-day service period**.
The service runs **12 hours per day** and costs **$50 per day**.

During the month, outages occurred:

* 30 minutes
* 2 hours
* 1 hour 30 minutes
* 45 minutes

### Service Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99%          | 10%    |
| < 98%          | 25%    |

### Tasks

1. Calculate **total downtime**
2. Calculate **actual availability**
3. Check **SLA violation**
4. Determine **service credit**
5. Calculate **final payable amount**

---

# 2️⃣ SaaS Platform Case

A SaaS company guarantees **99.5% availability** for **30 days**.
The service operates **8 hours per day** and costs **$35 per day**.

Outages recorded:

* 40 minutes
* 1 hour
* 1 hour 20 minutes

### Service Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.5%        | 10%    |
| < 99%          | 20%    |

### Tasks

1. Total downtime
2. Actual availability
3. SLA violation check
4. Service credit
5. Final payment

---

# 3️⃣ Cloud Storage SLA

A cloud storage provider guarantees **99.8% availability** for **28 days**.
Service runs **24 hours per day** and costs **$60 per day**.

Outages recorded:

* 1 hour
* 1 hour 30 minutes
* 2 hours

### Service Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.8%        | 10%    |
| < 99.5%        | 20%    |

### Tasks

1. Calculate downtime
2. Calculate actual uptime
3. Determine SLA violation
4. Determine service credit
5. Calculate final cost

---

# 4️⃣ Banking Cloud System

A bank signs an SLA guaranteeing **99.9% availability** for **30 days**.
Service operates **24 hours per day** and costs **$100 per day**.

Outages:

* 20 minutes
* 30 minutes
* 1 hour
* 40 minutes

### Service Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.9%        | 15%    |
| < 99%          | 30%    |

### Tasks

1. Total downtime
2. Actual availability
3. SLA violation
4. Service credit
5. Final payable amount

---

# 5️⃣ Video Streaming Platform

A streaming service guarantees **99.7% availability** for **30 days**.
The service runs **18 hours per day** and costs **$70 per day**.

Outages:

* 1 hour
* 2 hours
* 45 minutes

### Service Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.7%        | 10%    |
| < 99.3%        | 20%    |

### Tasks

Same 5 tasks.

---

# 6️⃣ Online Learning Platform

A cloud LMS guarantees **99.5% availability** for **28 days**.
Service operates **12 hours per day** and costs **$45 per day**.

Outages:

* 1 hour
* 1 hour 15 minutes
* 2 hours
* 30 minutes

### Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.5%        | 10%    |
| < 99%          | 25%    |

### Tasks

Same 5 calculations.

---

# 7️⃣ E-Commerce Cloud SLA

An e-commerce company signs an SLA guaranteeing **99.9% availability** for **30 days**.
Service operates **24 hours per day** and costs **$120 per day**.

Outages:

* 50 minutes
* 1 hour
* 1 hour 30 minutes

### Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.9%        | 10%    |
| < 99.5%        | 20%    |

### Tasks

Same 5 calculations.

---

# 8️⃣ Healthcare Cloud Service

A hospital uses a cloud system with **99.95% availability** for **30 days**.
Service runs **24 hours per day** and costs **$150 per day**.

Outages:

* 30 minutes
* 20 minutes
* 40 minutes

### Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.95%       | 10%    |
| < 99.8%        | 20%    |

### Tasks

Same 5 tasks.

---

# 9️⃣ Mobile App Backend SLA

A mobile company signs an SLA guaranteeing **99.6% availability** for **30 days**.
Service runs **16 hours per day** and costs **$80 per day**.

Outages:

* 1 hour
* 45 minutes
* 30 minutes
* 2 hours

### Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.6%        | 10%    |
| < 99.2%        | 20%    |

---

# 10 FinTech Cloud SLA

A fintech startup signs an SLA guaranteeing **99.9% availability** for **28 days**.
Service operates **12 hours per day** and costs **$90 per day**.

Outages:

* 1 hour
* 2 hours
* 30 minutes
* 1 hour 30 minutes

### Credit Policy

| Monthly Uptime | Credit |
| -------------- | ------ |
| < 99.9%        | 10%    |
| < 99.5%        | 25%    |


