# snmp_rs

[![Crates.io](https://img.shields.io/crates/v/snmp_rs.svg)](https://crates.io/crates/snmp_rs)
[![Docs.rs](https://docs.rs/snmp_rs/badge.svg)](https://docs.rs/snmp_rs)

**snmp_rs** is a pure-Rust SNMP library that aims to provide a complete, efficient, and extensible implementation of the Simple Network Management Protocol.  

This project is forked from [hroi/rust-snmp](https://github.com/hroi/rust-snmp) and extended with the goal of supporting modern features such as SNMPv3 (USM/VACM), trap/inform send & receive, and bulk/walk helpers.  

---

## Features (planned & in progress)

- SNMP v1 / v2c client operations  
  - get, get_next, set  
- High-level operations  
  - get_bulk, walk(), table()  
- Trap & Inform  
  - Trap receive (listener)  
  - Trap/Inform send  
- SNMPv3  
  - USM authentication & privacy (MD5, SHA, AES, DES)  
  - VACM access control  
- Pluggable transports  
  - std::net::UdpSocket (blocking)  
  - tokio::net::UdpSocket (async)  
- Zero-copy BER/ASN.1 encoder & decoder  
