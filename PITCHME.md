### SRE in Scalar (2020-1Q)
　  
　  
　  
　  
　　　id:tei-k
---

### Mission
- Paying off technical debt! |
- Migration to Azure |
- Easy to use orchestration tool to partners and Scalar delivery team |
- Enhancements |
- Make yourself confident of Infra orchestration and operations |

---

### Paying off technical debt!
- Scalar deployment can be broken up into loosely coupled modules |
- C* can be automatically started when deployed |
- Scalar cluster can be deployed simply |
- Jenkins-based CI and workflows are migrated into GitHub |
- Time for the end to end testing with terratest is reduced |
- Disk handling for cloud providers are more maintainable |

---

### Migration to Azure
- Production-simulated testing is running in Azure |
- Sandbox is running with the orchestration tool and Scalar DLT in Azure |

---

### Easy to use orchestration tool to partners and Scalar delivery team
- Terraform itself and its modules are upgraded to the newest version |
- The docs are updated and organized and easier to follow by partners |
- The tool is publicly available under Apache 2 license |

---

### Enhancements
- Scheduled operations can be configured easily (with k8s or Rundeck) |
- A customized docker cluster can be deployed and managed (with k8s) |
- (STRETCH) Stateless servers can be deployed and managed with k8s |

---

### Make yourself confident of Infra orchestration and operations
- Regular normal case operations (upgrade scalardl, backup, repair, ...) are conducted in the production-simulated testing environment |
- Destructive testing is conducted regularly |

---

### What are your impactful contributions to Scalar in the last Quarter?
- 1. New design for Orchestration Tool |
- 2. CI Test in Github Actions for Terraform |
- 3. Display correct status in Prometheus |

---

### 1. New design for Orchestration Tool
https://github.com/scalar-labs/scalar-terraform

---

### Current
- Directory structure |
```
- main -> module (bai, chiku, sho)
- module(bai, chiku, sho) -> module(base)
- module (base) -> moudle(network), module(cassandra), module(scalardl),module(monitor),...
- module(scalardl) -> module(universal)
```

---

![](https://i.imgur.com/62V9bsp.jpg)

---

### New Design
- Directory structure |
```
- network -> module(network) -> module(universal)
- cassandra -> module(cassandra) -> module(universal)
- scalardl -> module(scalardl) -> module(universal)
- monitor -> module(monitor) -> module(universal)
```

---

![](https://i.imgur.com/Jm8N6hk.jpg)

---

### Improvement Effect
- Simply |
- Maintenable |

---

### 2. Correct status in Prometheus

---

### Before
![](https://i.imgur.com/1cXVUpu.png)


---

### After1
![](https://i.imgur.com/dMD3EVj.png)

---

### After2
![](https://i.imgur.com/cSkD2op.png)

---

### 3. CI Test in Github Actions for Terraform

---

- terraform [fmt|validate|plan] |
- ![](https://i.imgur.com/OuhGtbs.png) |

---

### Next Action

---

### 1. Terratest in Github Actions (AWS/Azure)

---

Daily Integration Test (everyday 9:00 JST)

---

### 2. Create new documents

---

### 3. Pre Release

---

### 4. Make Repository to public

---
