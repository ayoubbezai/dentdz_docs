# 🦷 dentdz - Complete Features Documentation

> **dentdz** is a comprehensive dental management SaaS platform designed to streamline clinic operations, patient management, and administrative tasks for dental practices of all sizes.

**Last Updated:** May 2026  
**Version:** 2.0

---

## 📑 Table of Contents

1. [Language Support](#-language-support)
2. [Pricing Model](#-pricing-model)
3. [User Roles & Permissions](#-user-roles--permissions-system)
4. [Core Features](#-core-features-overview)
5. [Patient Management](#-patient-management-system)
6. [Procedures & Treatment Plans](#-procedures--treatment-plans)
7. [Invoice & Billing](#-invoice--billing-system)
8. [Patient Portal](#-patient-portal)
9. [Analytics & Reports](#-analytics--reports)
10. [Additional Features](#-additional-features)

---

## 🌍 Language Support

- ✅ **English** - Full support
- ✅ **French** - Full support  
- ✅ **Arabic** - Full support

All interfaces, reports, prescriptions, and patient portal support multi-language functionality.

---

## 💰 Pricing Model

### Simple, Transparent Pricing

**No subscription tiers - Pay only for what you use:**

- **Clinic Account:** 1,800 DA/month
  - Includes one clinic owner account
  - Full access to all features
  - Unlimited patients
  - All analytics modules
  - Patient portal included
  - 21+ prescription templates
  
- **Additional Staff:** 1,000 DA/month per staff member
  - Add dentists, receptionists, assistants
  - Each staff member gets their own account
  - Customizable permissions per staff
  - No limit on number of staff

**Example Pricing:**
- Solo practitioner: 1,800 DA/month
- Clinic with 2 dentists + 1 receptionist: 1,800 + (3 × 1,000) = 4,800 DA/month
- Large clinic with 5 staff members: 1,800 + (5 × 1,000) = 6,800 DA/month

**All Features Included:**
- ✅ Unlimited patients
- ✅ All analytics (5 modules)
- ✅ Patient portal
- ✅ Invoice system
- ✅ 21+ prescription templates
- ✅ Inventory management
- ✅ Lab management
- ✅ Audit logs
- ✅ Multi-account switching
- ✅ Export (CSV/PDF)
- ✅ Email support

---

## 🔐 User Roles & Permissions System

dentdz implements a **granular permission-based access control system** with **40+ specific permissions**. Each user can have multiple permissions assigned individually.

### Role Overview

| Role | Typical Access | Primary Use Case |
|------|---------------|------------------|
| 🏥 **Clinic Owner** | Full Administrative | Complete control over clinic, staff, and settings |
| 🦷 **Dentist** | Full Clinical | All clinical and management features |
| 👔 **Receptionist** | Front Desk | Patient registration, appointments, billing |
| 🤝 **Assistant** | Clinical Support | Support dentists with procedures and documentation |
| 👨‍💼 **Super Admin** | Platform Level | SaaS platform management (dentdz team only) |

### Permission Categories (40+ Permissions)

The system uses granular permissions for each module:

#### 1. **Patient Management** (4 permissions)
- `can_view_patient` - View patient list and details
- `can_create_patient` - Register new patients
- `can_update_patient` - Edit patient information
- `can_delete_patient` - Remove patients

#### 2. **Appointments** (4 permissions)
- `can_view_appointment` - View appointments
- `can_create_appointment` - Schedule appointments
- `can_update_appointment` - Modify appointments
- `can_delete_appointment` - Cancel appointments

#### 3. **Treatment Plans Catalog** (4 permissions)
- `can_view_treatment_plan` - View procedure catalog
- `can_create_treatment_plan` - Create procedure templates
- `can_update_treatment_plan` - Edit templates
- `can_delete_treatment_plan` - Remove templates

#### 4. **Procedures** (4 permissions)
- `can_view_procedure_item` - View patient procedures
- `can_create_procedure_item` - Add procedures
- `can_update_procedure_item` - Edit procedures
- `can_delete_procedure_item` - Remove procedures

#### 5. **Invoices & Payments** (4 permissions)
- `can_view_invoice` - View invoices
- `can_create_invoice` - Generate invoices
- `can_view_patient_payment` - View payments
- `can_create_patient_payment` - Record payments

#### 6. **Prescriptions** (4 permissions)
- `can_view_prescription` - View prescriptions
- `can_create_prescription` - Create prescriptions
- `can_update_prescription` - Edit prescriptions
- `can_delete_prescription` - Remove prescriptions

#### 7. **Documents** (3 permissions)
- `can_view_document` - View documents
- `can_create_document` - Upload documents
- `can_delete_document` - Remove documents

#### 8. **Inventory** (11 permissions)
- Stock: `can_view_stock`, `can_create_stock`, `can_update_stock`, `can_delete_stock`
- Suppliers: `can_view_supplier`, `can_create_supplier`, `can_update_supplier`, `can_delete_supplier`
- Logs: `can_view_stock_logs`
- Notifications: `can_view_stock_notification`

#### 9. **Laboratory** (8 permissions)
- Labs: `can_view_lab`, `can_create_lab`, `can_update_lab`, `can_delete_lab`
- Lab Works: `can_view_lab_work`, `can_create_lab_work`, `can_update_lab_work`, `can_delete_lab_work`

#### 10. **Medicines** (4 permissions)
- `can_view_medicine`, `can_create_medicine`, `can_update_medicine`, `can_delete_medicine`

#### 11. **Staff Management** (4 permissions)
- `can_view_staff`, `can_create_staff`, `can_update_staff`, `can_delete_staff`

#### 12. **Clinic Expenses** (4 permissions)
- `can_view_clinic_expense`, `can_create_clinic_expense`, `can_update_clinic_expense`, `can_delete_clinic_expense`

#### 13. **Analytics** (6 permissions)
- `can_view_analytics` - General analytics access
- `can_view_patient_analytics` - Patient statistics
- `can_view_financial_analytics` - Financial reports
- `can_view_appointment_analytics` - Appointment analytics
- `can_view_medical_analytics` - Medical analytics
- `can_view_stock_analytics` - Inventory analytics

#### 14. **Settings** (4 permissions)
- `can_manage_patient_portal_settings` - Configure patient portal
- `can_manage_prescription_settings` - Configure prescriptions
- `clinic_account` - Clinic owner marker
- `staff_account` - Staff member marker

#### 15. **Support & Portal** (4 permissions)
- `can_view_support`, `can_create_support`
- `can_view_patient_portal`, `can_create_patient_portal`

#### 16. **Platform Admin** (1 permission)
- `super_admin` - Full platform access (dentdz team only)

### Typical Permission Sets by Role

#### 🏥 Clinic Owner
**Full access to everything:**
- All staff management permissions
- All settings permissions
- Full access to analytics
- Full access to all clinical features
- Can manage patient portal settings
- Can manage prescription settings

#### 🦷 Dentist
**Full clinical access:**
- Full patient management (view, create, update, delete)
- Full appointments
- Full procedures and treatment plans
- Full prescriptions
- Full invoices and payments
- Full documents
- Full analytics
- View-only staff access
- No staff management

#### 👔 Receptionist
**Front desk operations:**
- Patient: view, create, update (no delete)
- Appointments: full access
- Payments: view, create
- Invoices: view, create
- Documents: view, create
- Limited patient tab access (no prescriptions, no procedures)

#### 🤝 Assistant
**Clinical support:**
- Patient: view only
- Appointments: view, create, update
- Procedures: view
- Prescriptions: view
- Documents: view, create
- No billing/payment access
- No invoice access

---

## 🎯 Core Features Overview

### 📊 Dashboard & Overview
- **Real-time Statistics** - Today's appointments, payments, key metrics
- **Quick Actions** - Fast access to common tasks
- **Appointment Graph** - Visual appointment trends
- **Payment Summary** - Today's payment overview
- **Notifications** - Stock alerts and system notifications

---

## 👨‍⚕️ Patient Management System

### Patient List
- 📋 **Complete Patient Directory** - Searchable and filterable
- 🔍 **Advanced Search** - Find by name, phone, email
- 📊 **Patient Statistics** - Total patients, demographics
- ➕ **Quick Registration** - Fast patient onboarding
- 📤 **Export** - CSV and PDF export

### Patient Profile - New Simplified Structure

**All patient information is now in ONE place - the patient details page.**

When you open a patient, you see a comprehensive profile with **7 tabs:**

#### Available Tabs:

1. **📋 Procedures** (Default Tab)
   - All dental procedures for this patient
   - Visual tooth chart (odontogram)
   - Add procedures from treatment plan catalog
   - Track procedure status (Planned, In Progress, Completed, Cancelled)
   - Specify tooth numbers
   - Set prices and notes

2. **📅 Appointments**
   - All patient appointments
   - Schedule new appointments
   - Assign dentist
   - Set status
   - Add notes

3. **🧾 Invoices**
   - All patient invoices
   - Create invoices from procedures
   - Track payment status
   - Apply discounts
   - View invoice details

4. **💊 Prescriptions**
   - All prescriptions for patient
   - Create new prescriptions
   - 21+ professional templates
   - Multi-language support
   - Download PDF

5. **📁 Documents**
   - Upload patient files
   - X-rays, medical records
   - Treatment plans
   - Download and manage files

6. **🔬 Lab Orders**
   - Laboratory work orders
   - Track lab work status
   - Link to specific procedures
   - Manage delivery dates

7. **💳 Payments**
   - All payment history
   - Record new payments
   - Link payments to invoices
   - Track payment methods

### Patient Header Information

**Displayed at top of patient profile:**
- Patient photo
- Name, age, gender
- Contact information (phone, email)
- Medical history summary
- Allergies
- Current medications
- Quick action buttons

### Dental Chart (Odontogram)

**Interactive visual tooth chart:**
- Shows all procedures on teeth
- Color-coded by status
- Click tooth to see procedures
- Visual representation of dental work
- Multiple odontogram layouts available

### Patient Information Sections

**Basic Information:**
- First name, last name
- Date of birth (auto-calculates age)
- Gender
- Patient photo
- Phone number
- Email address
- Physical address
- General notes

**Medical Information:**
- Medical conditions
- Current medications
- Allergies
- Medical history notes

### Tab Access Control

**Role-based tab visibility:**

- **Clinic Owner/Dentist:** All 7 tabs visible
- **Receptionist:** Only Appointments, Invoices, Payments (no clinical tabs)
- **Assistant:** Only Appointments, Prescriptions, Documents (no billing)

---

## 🦷 Procedures & Treatment Plans

### Treatment Plans (Procedure Catalog)

**Location:** `/treatment-plans` page

**Purpose:** Create a catalog of procedures your clinic offers

**Features:**
- ➕ **Create Templates** - Define standard procedures
- 📝 **Details** - Name, code, description, category
- 💰 **Default Pricing** - Set standard prices
- ⏱️ **Duration** - Estimated time
- 🏷️ **Categories** - Organize by type
- ✅ **Active/Inactive** - Enable/disable procedures

**Categories:**
- Preventive (Cleaning, Checkup, Fluoride)
- Restorative (Filling, Crown, Bridge)
- Cosmetic (Whitening, Veneer)
- Orthodontic (Braces, Retainer)
- Surgical (Extraction, Implant)
- Endodontic (Root Canal)
- Periodontic (Gum Treatment)
- Pediatric (Children's Dentistry)

**Example Treatment Plans:**
- Dental Cleaning - 2,000 DA - 30 minutes
- Root Canal - 15,000 DA - 90 minutes
- Crown Placement - 25,000 DA - 60 minutes
- Teeth Whitening - 10,000 DA - 45 minutes

### Procedure Items (Patient Procedures)

**Location:** Patient Profile → Procedures Tab

**Purpose:** Track actual procedures performed on patients

**Workflow:**
1. Open patient profile
2. Go to Procedures tab
3. Click "Add Procedure"
4. Select from treatment plan catalog (or create custom)
5. Specify tooth number (if applicable)
6. Set price (defaults from catalog)
7. Set status
8. Add notes

**Procedure Statuses:**
- 🟡 **Planned** - Scheduled for future
- 🔵 **In Progress** - Currently being performed
- 🟢 **Completed** - Finished
- 🔴 **Cancelled** - Not performed

**Visual Tooth Chart:**
- Interactive odontogram
- Color-coded by status
- Click tooth to see procedures
- Multiple layout options

---

## 🧾 Invoice & Billing System

### Invoice Generation

**Location:** Patient Profile → Invoices Tab

**Features:**
- 📄 **Unique Invoice Numbers** - Auto-generated
- 📋 **Invoice Items** - Link procedures to invoices
- 💰 **Pricing** - Individual item pricing
- 🏷️ **Discounts** - Per item or total
- 🧮 **Automatic Calculations** - Total, discount, final amount
- 💳 **Payment Tracking** - Paid vs total
- 📊 **Status** - Unpaid, Partially Paid, Paid

**Invoice Workflow:**
1. Go to patient → Invoices tab
2. Click "Create Invoice"
3. Select procedures to include
4. Set prices and discounts
5. Generate invoice
6. Record payments

**Invoice Details:**
- Invoice number
- Date
- Patient information
- Procedure list
- Prices and discounts
- Total amount
- Paid amount
- Balance due
- Status

### Payment Recording

**Two Types:**
1. **Invoice Payments** - Linked to invoices
2. **General Payments** - Not linked to invoices

**Payment Information:**
- Amount
- Payment method
- Payment date
- Notes
- Invoice reference (if applicable)

**Payment Methods:**
- 💵 Cash
- 💳 Credit/Debit Card
- 🏦 Bank Transfer
- 📝 Check
- 🔄 Other

### Clinic Expenses

**Location:** `/payments` page → Clinic Expenses tab

**Track operational costs:**
- 🏢 Rent
- 💡 Utilities
- 🔧 Equipment
- 📦 Supplies
- 💼 Salaries
- 📱 Marketing
- 🔄 Other

---

## 🌐 Patient Portal

**Separate web application for patients**

### Overview

The Patient Portal is a **separate Next.js application** allowing patients to access their dental records securely.

**Access Method:**
- Clinic generates unique access token
- Token sent to patient
- Patient visits portal URL with token
- Secure, time-limited access

### Portal Features (Configurable)

Clinic owners enable/disable each feature:

#### ✅ View Appointments
- Past and upcoming appointments
- Date, time, status
- Dentist assigned
- Notes

#### ✅ View Invoices
- All invoices
- Invoice details
- Amount due
- Payment status

#### ✅ View Payments
- Payment history
- Amounts and methods
- Payment dates

#### ✅ View Procedures
- All procedures performed
- Tooth numbers
- Status and dates

#### ✅ View Prescriptions
- All prescriptions
- Medications
- Dosage instructions
- Download PDFs

#### ✅ View Documents
- Uploaded documents
- Medical records
- X-rays
- Download files

### Portal Configuration

**Location:** Settings → Patient Portal Settings

**Settings:**
- Enable/disable portal
- Toggle individual features
- Set token expiration
- Configure permissions

**Security:**
- Unique tokens per patient
- Token expiration
- Last used tracking
- Read-only access

---

## 📊 Analytics & Reports

### 5 Analytics Modules

**Comprehensive analytics with 20+ charts:**

#### 1. 💰 Financial Analytics

**Charts:**
- Revenue vs Expenses
- Monthly revenue trends
- Payment method distribution
- Revenue by procedure type
- Expense breakdown
- Profit margins

**Metrics:**
- Total revenue
- Total expenses
- Net profit
- Average transaction
- Growth rate

#### 2. 👥 Patient Analytics

**Charts:**
- Patient growth
- Age distribution
- Gender distribution
- Visit frequency
- New vs returning
- Retention rate

**Metrics:**
- Total patients
- New patients
- Active patients
- Demographics
- Average visits

#### 3. 📅 Appointment Analytics

**Charts:**
- Appointment growth
- Status distribution
- By dentist
- By day of week
- By time slot
- Cancellation rate

**Metrics:**
- Total appointments
- Completed
- Cancelled
- Pending
- Average per day

#### 4. 🏥 Medical Analytics

**Charts:**
- Procedures by category
- Most common procedures
- Completion rates
- Treatment duration
- Success rates

**Metrics:**
- Total procedures
- By type
- Average cost
- Completion rate

#### 5. 📦 Stock Analytics

**Charts:**
- Stock levels
- Low stock items
- Medicine expiry timeline
- Usage trends
- Supplier performance

**Metrics:**
- Total stock items
- Low stock alerts
- Expiring items
- Stock value

### Report Generation

**Export Capabilities:**
- 📄 **PDF Reports** - Professional formatted
- 📊 **CSV Export** - Data analysis
- 📅 **Date Range** - Custom periods
- 🎯 **Filtered Reports** - Export filtered data

**Exportable Entities:**
- Patients
- Appointments
- Payments
- Invoices
- Procedures
- Prescriptions
- Stock items
- Lab works
- Medicines
- Staff
- Clinic expenses
- Suppliers

---

## 📅 Appointments

### Two Views

1. **Table View** - List of all appointments
2. **Calendar View** - Visual calendar

### Appointment Features

**Information:**
- Patient name
- Dentist assigned
- Date and time
- Duration
- Status
- Notes

**Statuses:**
- 🟡 Pending
- 🟢 Confirmed
- 🔵 In Progress
- ✅ Completed
- 🔴 Cancelled
- ⚠️ No Show

**Calendar Features:**
- Monthly/weekly/daily views
- Drag and drop
- Color-coded by status
- Dentist filtering
- Quick creation

---

## 💊 Prescriptions

### 21+ Professional Templates

**Prescription Features:**
- Patient details
- Prescription date
- Medication list
- Doctor information
- Clinic branding

**Medication Details:**
- Medicine name
- Dosage
- Frequency
- Times per day
- Quantity
- Route
- Instructions

### Prescription Settings

**Location:** Settings → Prescription Settings

**Configurable:**
- Clinic name (FR/AR)
- Clinic address (FR/AR)
- Clinic phone
- Clinic logo
- Doctor name (FR/AR)
- Doctor specialty (FR/AR)
- Preferred template

**PDF Generation:**
- Professional output
- Clinic branding
- Multi-language
- Downloadable

---

## 📦 Inventory Management

### Stock Management

**Stock Details:**
- Item name
- Category
- Current quantity
- Reorder point
- Unit
- Expiry date
- Supplier
- Status

### Stock Notifications

**Automatic Alerts:**
- ⚠️ Low Stock
- 📅 Expiring Soon
- 🔴 Expired

### Stock Logs

**Audit Trail:**
- All changes tracked
- User who made change
- Previous/new quantity
- Date and time

### Suppliers

**Supplier Directory:**
- Name
- Specialty
- Phone numbers
- Email
- Notes

---

## 🔬 Laboratory Management

### Lab Directory

**Lab Information:**
- Lab name
- Specialty
- Contact details
- Notes

### Lab Works

**Lab Order Details:**
- Lab name
- Item type
- Patient linked
- Send/return dates
- Status
- Price
- Notes

**Statuses:**
- 📤 Sent
- 🔄 In Progress
- ✅ Completed
- 📥 Delivered

---

## 💊 Medicine Database

**Quick reference for prescriptions:**
- Medicine name
- Category
- Quantity/strength
- Notes
- Usage instructions

**Integration:**
- Quick search in prescriptions
- Auto-complete
- Standard dosages

---

## 👥 Staff Management

**Staff Features:**
- Personal information
- Photo
- Phone number
- Specialty
- User account
- Notes

**Permission Assignment:**
- 40+ individual permissions
- Custom permission sets
- Permission explanations

**Staff Statistics:**
- Appointments handled
- Patients seen
- Procedures performed

---

## 📁 Document Management

**Global document storage:**
- Upload files
- Organize by patient
- File types: PDF, images, documents
- Search and filter
- Download files

---

## 📜 Audit Log

**System-wide activity tracking:**

**Logged Information:**
- Operation type
- User who performed action
- Table/entity affected
- Record ID
- Previous/new data
- IP address
- Timestamp

**Use Cases:**
- Security auditing
- Compliance tracking
- Error investigation
- User activity monitoring

---

## 🔄 Multi-Account Session Switching

**Manage multiple clinic accounts:**

**Use Case:** Users working at multiple clinics

**Features:**
- Add multiple accounts
- Switch without re-login
- Session management
- Account list in menu

---

## 🆘 Support System

**Support Tickets:**
- Create tickets
- Title and description
- Priority levels
- Type selection
- File attachments
- Status tracking

---

---

## 📞 Support & Contact

**Support Channels:**
- 📧 Email: dentdzapp@gmail.com
- 💬 In-App Support: Through support page
- 📚 Documentation: Comprehensive guides

**Support Hours:**
- Email support (24-48h response)

---

**Made with ❤️ for Dental Professionals**

*Simplifying dental practice management, one clinic at a time.*

© 2026 dentdz. All rights reserved.
