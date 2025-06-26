# Laptop-request-catalog-item-
# **Laptop Request Catalog Item**  
*Streamline employee laptop requests through a standardized process.*  

## **Description**  
This catalog item enables employees to request laptops (new, replacement, or upgrade) via the company's IT service management system (e.g., ServiceNow, Jira).  

---

## **Request Form Fields**  
| Field               | Type          | Required? | Notes                          |  
|---------------------|---------------|-----------|--------------------------------|  
| **Requester Name**  | Text          | Yes       | Auto-filled if logged in.      |  
| **Department**      | Dropdown      | Yes       | Finance, Engineering, HR, etc.|  
| **Laptop Model**    | Dropdown      | Yes       | MacBook Pro, Dell XPS, etc.    |  
| **Configuration**   | Checkboxes    | No        | RAM (16GB/32GB), Storage (512GB/1TB), etc. |  
| **Justification**   | Text Area     | Yes       | "New hire," "Hardware failure," etc. |  
| **Urgency**        | Radio Buttons | No        | Low/Medium/High                |  

---

## **Approval Workflow**  
1. **Submission**: Employee fills out the form.  
2. **Manager Approval**: Request routed to the requester's manager.  
3. **IT Review**: IT verifies inventory/compatibility.  
4. **Fulfillment**:  
   - Standard models: Delivered in **3–5 business days**.  
   - Custom orders: **1–2 weeks**.  

---

## **Integration Requirements**  
- Syncs with **Active Directory** for user/department data.  
- Connects to **inventory management** (e.g., SNOW, Asset Tiger).  
- Email notifications via **SMTP**.  

---

## **How to Update**  
1. Edit the catalog item in `service-now/admin` (for ServiceNow).  
2. Modify dropdown options in `config/laptop_models.json`.  

---

## **Troubleshooting**  
| Issue                     | Solution                          |  
|---------------------------|-----------------------------------|  
| Missing manager approval  | Check AD group mappings.          |  
| Incorrect model options   | Update `laptop_models.json`.      |  

---

**Questions?** Contact IT Support at `it-support@company.com`.  

---

### **Formatting Notes**  
- Save this as `README.md` for proper Markdown rendering.  
- Use tables for clear field/workflow documentation.  
- Adjust sections based on your tools (e.g., ServiceNow, Jira, custom ERP).  
-
