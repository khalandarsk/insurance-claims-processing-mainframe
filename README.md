# Insurance Claims Processing System (Mainframe)

This project demonstrates a batch-based Insurance Claims Processing System
implemented on IBM Mainframe using COBOL, VSAM, DB2, and JCL.

The system processes daily insurance claim transactions, validates them against
policy master data, stores complete claim history for audit and compliance,
updates policy balances for approved claims, and generates reject files for
invalid claims.

---

## 📁 Project Structure


insurance-claims-processing-mainframe/
├── README.md
│
├── sample-data/
│   ├── policy_input.ps
│   └── claim_input.ps
│
├── vsam/
│   └── policy_master.idcams
│
├── jcl/
│   ├── JOBPOL01.jcl
│   ├── JOBCLM01.jcl
│   └── JOBUPD01.jcl
│
├── db2/
│   ├── claim_history.sql
│   └── policy_table.sql
│
├── dclgen/
│   └── CLAIMH.cpy
│
├── cobol/
│   ├── COBCLM01.cbl
│   └── COBUPD01.cbl
│
└── optional/
    └── cobol/
        └── COBPOL01_FIELD_COPY.cbl

## 🔄 Flow
- Policy input is loaded into VSAM master
- Daily claim input is validated against policy master
- All claims (approved/rejected) are stored in DB2
- Approved claims update policy balance
- Rejected claims are written to a reject file


## 🛠️ Technologies
COBOL, VSAM KSDS, DB2, JCL, IDCAMS REPRO, DCLGEN

## 👨‍💻 Experience Level
Designed and implemented at a **2-year mainframe batch developer level**.

## 🔁 Optional Enhancement
An optional COBOL program is provided to demonstrate field-by-field
policy master loading when validation or layout changes are required.
