# 🏥 Hospital Management Database  

## 🎯 Objective  
A SQL-based project designed to manage **patients, doctors, visits, billing, and reports** in a hospital.  

## 📂 Repository Contents  
- **hospital_management.sql** → Full SQL (schema + sample data + functions + triggers + reports)  
- **hospital_schema.sql** → Database schema only  
- **hospital_functions.sql** → Stored procedure & function  
- **hospital_triggers.sql** → Triggers for patient discharge & billing update  
- **hospital_reports.sql** → SQL queries for reporting  
- **hospital_reports.xlsx** → Reports in Excel format  
- **hospital_reports.pdf** → Reports in PDF format  

## 🛠️ Tools  
- MySQL (or MariaDB)  
- DBeaver / MySQL Workbench  
- Python (for generating Excel/PDF reports)  

## 🚀 Features  
1. **Schema**: Patients, Doctors, Visits, Bills.  
2. **Sample Data**: Preloaded example records.  
3. **Stored Procedure**: `GetTotalBillByName` – retrieves the total bill for a patient.  
4. **Stored Function**: `GetOutstandingBalanceByName` – calculates outstanding balance.  
5. **Triggers**:  
   - `trg_discharge_update` → updates status when a patient is discharged.  
   - `trg_payment_update` → updates bill status when payment is made.  
6. **Reports**:  
   - Patient visit history  
   - Doctor’s appointments  
   - Billing summary  

## 📊 Sample Reports (Generated from SQL)  
- **Excel** → [hospital_reports.xlsx](hospital_reports.xlsx)  
- **PDF** → [hospital_reports.pdf](hospital_reports.pdf)  

## 📌 Usage  
1. Import `hospital_management.sql` into MySQL.  
2. Run schema and sample inserts.  
3. Example calls:  
   ```sql
   CALL GetTotalBillByName('Alice Smith');
   SELECT GetOutstandingBalanceByName('Alice Smith');