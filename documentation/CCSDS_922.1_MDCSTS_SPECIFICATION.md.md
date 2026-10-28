# CCSDS 922.1-B-2 Monitored Data Service (MD-CSTS) Specification

**Document**: CCSDS 922.1-B-2 (Blue Book, Issue 2, September 2022\)  
**Framework**: CCSDS 921.1-B-2 (Cross Support Transfer Services — Specification Framework)  
**System**: MDCSTSForge Pro (v1.0.0)

## 1\. Executive Summary & Architectural Scope

CCSDS 922.1-B-2 defines the Monitored Data Service (MD-CSTS), a standardized cross-support transfer service within the CCSDS CSTS framework. It enables a spacecraft Mission Operations Center (the User, such as NASA AMMOS, ESA ESOC, JAXA) to monitor in real-time or retrieve from archive the status, operational parameters, and physical telemetry of an external ground station tracking network (the Provider, such as NASA DSN, ESA ESTRACK, KSAT, SSC).

## 2\. Service Architecture & State Machine

- State Transitions (§3.2): State 1 (UNBOUND) \-\> State 2 (READY) \-\> State 3 (ACTIVE).  
- Core Operations: BIND, UNBIND, START, STOP, TRANSFER-DATA, NOTIFY.  
- Telemetry Parameters: Carrier lock, symbol SNR (Eb/N0), antenna azimuth/elevation angles, uplink transmitter power, Doppler residual, and receiver AGC.