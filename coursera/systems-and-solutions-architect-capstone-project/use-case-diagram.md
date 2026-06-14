使用案例圖的核心就是：

先找出系統外的 **actors**，
再找出系統內的 **use cases**，
最後說明彼此的互動關係 。

---

***

## 1. Identify the actors

| Actor | Primary/Secondary | Role | Interactions |
|---|---|---|---|
| Customer | Primary | 銀行數位平台的最終使用者 | 提交 KYC 資料、開戶、查看帳戶、執行交易 |
| Product Owner | Primary | 定義業務規則與功能需求 | 設定貸款流程、監控 fraud alerts、調整業務規則 |
| Compliance Officer | Primary | 確保系統符合監管與內控要求 | 檢查 audit logs、KYC reports、合規設定 |
| DevOps Engineer | Primary | 管理部署、測試與維運流程 | 執行 CI/CD、監控部署、處理 rollback |
| Regulator | Secondary | 外部監管單位 | 查看合規報告與稽核資料 |
| Payment Gateway | Secondary | 外部付款系統 | 處理交易授權與回傳結果 |
| Credit Bureau API | Secondary | 外部信用資料系統 | 提供信用查詢與風險評估結果 |

***

## 2. Define the use cases

| Use case | Description |
|---|---|
| Onboard New Customer | Customer submits KYC information; the system validates identity and creates account access. |
| Manage Customer Account | Customer views account details, updates profile, and manages access. |
| Configure Compliance Rules | Compliance officer defines thresholds and compliance settings for system-wide enforcement. |
| Access Audit Logs | Compliance officer views real-time audit logs and KYC reports. |
| Manage Deployment Pipeline | DevOps engineer triggers build, test, and deployment workflow. |
| Monitor Fraud Alerts | Product owner reviews fraud alerts and investigates suspicious events. |
| Access Regulatory Reports | Regulator securely accesses compliance and reporting information. |
| Process Payment Transaction | System communicates with payment gateway to authorize and complete payments. |
| Check Credit History | System requests customer credit information from credit bureau API for loan-related decisions. |
| Review Loan Application | Product owner reviews loan workflow results and applies approval rules. |

***

## 3. Use case diagram description

你在 Lucidchart 或 Draw.io 裡可以這樣畫：

### System boundary

畫一個大框，名稱可以寫：
**Core Digital Transformation Platform**

### Actors 放在框外

- Customer
- Product Owner
- Compliance Officer
- DevOps Engineer
- Regulator
- Payment Gateway
- Credit Bureau API

### Use cases 放在框內

- Onboard New Customer
- Manage Customer Account
- Configure Compliance Rules
- Access Audit Logs
- Manage Deployment Pipeline
- Monitor Fraud Alerts
- Access Regulatory Reports
- Process Payment Transaction
- Check Credit History
- Review Loan Application

***

## 4. 角色與 use case 的關係

| Actor | Use case | Relationship |
|---|---|---|
| Customer | Onboard New Customer | Direct interaction |
| Customer | Manage Customer Account | Direct interaction |
| Compliance Officer | Configure Compliance Rules | Direct interaction |
| Compliance Officer | Access Audit Logs | Direct interaction |
| DevOps Engineer | Manage Deployment Pipeline | Direct interaction |
| Product Owner | Monitor Fraud Alerts | Direct interaction |
| Product Owner | Review Loan Application | Direct interaction |
| Regulator | Access Regulatory Reports | Direct interaction |
| Payment Gateway | Process Payment Transaction | System-to-system interaction |
| Credit Bureau API | Check Credit History | System-to-system interaction |

***

## 5. 你可以直接放進模板的完整文字版

如果模板是要你一格一格填，你可以直接用下面這種格式：

### Actors

- **Customer** — Primary — Uses the digital banking platform to onboard, manage accounts, and perform transactions.
- **Product Owner** — Primary — Defines business rules and monitors fraud and loan workflows.
- **Compliance Officer** — Primary — Reviews audit logs, KYC reports, and compliance settings.
- **DevOps Engineer** — Primary — Manages build, test, deployment, and rollback processes.
- **Regulator** — Secondary — Reviews regulatory reports through secure access.
- **Payment Gateway** — Secondary — Supports payment authorization and transaction processing.
- **Credit Bureau API** — Secondary — Provides external credit data for loan-related checks.

### Use Cases

- **Onboard New Customer** — Customer submits KYC data; system validates identity and grants access.
- **Manage Customer Account** — Customer updates profile and views account details.
- **Configure Compliance Rules** — Compliance officer sets thresholds and policy rules.
- **Access Audit Logs** — Compliance officer reviews real-time logs and reports.
- **Manage Deployment Pipeline** — DevOps runs build, test, and deployment workflow.
- **Monitor Fraud Alerts** — Product owner reviews alerts and investigates suspicious activity.
- **Access Regulatory Reports** — Regulator securely views compliance reports.
- **Process Payment Transaction** — System processes payments through the gateway.
- **Check Credit History** — System queries credit bureau data for lending decisions.
- **Review Loan Application** — Product owner evaluates loan workflow results.

### Relationships

- Customer → Onboard New Customer, Manage Customer Account
- Compliance Officer → Configure Compliance Rules, Access Audit Logs
- DevOps Engineer → Manage Deployment Pipeline
- Product Owner → Monitor Fraud Alerts, Review Loan Application
- Regulator → Access Regulatory Reports
- Payment Gateway → Process Payment Transaction
- Credit Bureau API → Check Credit History

***

## 6. Reflection questions 可寫範例

### What challenges did you face when identifying actors and use cases?

The main challenge was separating internal users from external systems and ensuring each actor had a clear role in the banking workflow. Another challenge was keeping the use cases at the right level of detail without turning them into technical tasks.

### How does your diagram facilitate understanding of the program's functionality?

The diagram clearly shows which actors interact with which system functions, making the scope and responsibilities easier to understand. It also helps align business, compliance, and technical stakeholders around the same view of the system.

### What are your suggestions for improving customer experience?

Simplify the onboarding process, reduce response time, and provide clear real-time status updates. The platform should also improve self-service features and strengthen secure access to customer accounts.

***

## 7. 畫圖時的小提醒

- Actor 用人形或 stick figure 表示。
- Use case 用橢圓表示。
- 系統邊界用一個大方框包住 use cases。
- Actor 放在框外，use case 放在框內。
- 每條線表示互動關係，不必畫太複雜。
- 這次重點是「需求與互動」，不是畫得多花俏 。

