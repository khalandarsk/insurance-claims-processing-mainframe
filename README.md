# Insurance Claims Processing System (Mainframe)

This project demonstrates a batch-based Insurance Claims Processing System
implemented on IBM Mainframe using COBOL, VSAM, DB2, and JCL.

## Flow
- Policy input is loaded into VSAM master
- Daily claim input is validated against policy master
- All claims (approved/rejected) are stored in DB2
- Approved claims update policy balance
- Rejected claims are written to a reject file

## Technologies
COBOL, VSAM KSDS, DB2, JCL, IDCAMS REPRO, DCLGEN

## Experience Level
Designed and implemented at a 2-year mainframe batch developer level.

## Optional Enhancement
An optional COBOL program is provided to demonstrate field-by-field
policy master loading when validation or layout changes are required.
