## SRE in Scalar (20-1Q)
　  
　  


　　　2020.02.03

　　　id:@tei-k
---
### $WHOAMI

![](https://s.gravatar.com/avatar/6a288829cb26612a60633169a0ea480b.jpeg)

- Name: Kun Tei (@tei-k)
- Job: Freelance Engineer (SRE & Infrastructure)
- Language:
  - Terraform | Ansible | Docker | Packer | Python | Ruby | GO | ...
  - 🇨🇳🇯🇵🇰🇷...
- Join: 2019/12/02 〜 (Full Time)

---

## Mission
- 1️⃣Paying off technical debt! |
- 2️⃣Migration to Azure |
- 3️⃣Easy to use orchestration tool to partners and Scalar delivery team |
- 4️⃣Enhancements |
- 5️⃣Make yourself confident of Infra orchestration and operations |

---

### 1️⃣Paying off technical debt!
- Scalar deployment can be broken up into loosely coupled modules |
- C* can be automatically started when deployed |
- Scalar cluster can be deployed simply |
- Jenkins-based CI and workflows are migrated into GitHub |
- Time for the end to end testing with terratest is reduced |
- Disk handling for cloud providers are more maintainable |

---

### 2️⃣Migration to Azure
- Production-simulated testing is running in Azure |
- Sandbox is running with the orchestration tool and Scalar DLT in Azure |

---

### 3️⃣Easy to use orchestration tool to partners and Scalar delivery team
- Terraform itself and its modules are upgraded to the newest version |
- The docs are updated and organized and easier to follow by partners |
- The tool is publicly available under Apache 2 license |

---

### 4️⃣Enhancements
- Scheduled operations can be configured easily (with k8s or Rundeck) |
- A customized docker cluster can be deployed and managed (with k8s) |
- (STRETCH) Stateless servers can be deployed and managed with k8s |

---

### 5️⃣Make yourself confident of Infra orchestration and operations
- Regular normal case operations (upgrade scalardl, backup, repair, ...) are conducted in the production-simulated testing environment |
- Destructive testing is conducted regularly |

---

## Contributions 👷
- New design for Orchestration Tool |
- UP terraform version to latest with HCL2 |
- CI Test in Github Actions for Terraform |
- Integration Test in Github Actions with Terratest |
- Display correct status in Prometheus |

---

### 1. New design for Orchestration Tool ❇️
https://github.com/scalar-labs/scalar-terraform

---

#### Current
- main -> |
- module(bai, chiku, sho) -> |
- module (base) -> |
- module(scalardl) -> |
- module(universal) |

---

![](https://i.imgur.com/62V9bsp.jpg)

---

🤔
module.scalar.module.scalardl_bai.module.cassandra.module.cassandra_cluster.azurerm_resource_group.vm

---

#### New
- network -> |
- module (scalardl) -> |
- module (universal) |

---

![](https://i.imgur.com/Jm8N6hk.jpg)

---

![](https://i.imgur.com/xwZqXfQ.png)

---
😆
module.cassandra.module.cassy_cluster.azurerm_resource_group.vm

---

#### Improvement Effect
- Simply 🔰 |
- Maintenable 🏗 |
- Fastly 🚀 |

---

### 2. CI Test in Github Actions for Terraform

---

- terraform [ fmt | validate | plan ] |

---

![](https://i.imgur.com/OuhGtbs.png)

---

#### Improvement Effect

- Buity Code 🦋 |
- Check configuration 📝 |
- Dru-run ☑️ |

---

### 3. Integration Test in Github Actions with Terratest

---

- Terratest in Github Actions (Bye jenkins!) |
- Add terratest for Azure |
- Add testcase |

---

#### Improvement Effect
- Accuracy 🍀 |
- Fastly 🚀 |

---

![](https://i.imgur.com/pgrco9d.png)

---

### 4. Correct status in Prometheus

---

#### List of hosts (before)
![](https://i.imgur.com/1cXVUpu.png)


---

#### List of hosts (after)
![](https://i.imgur.com/dMD3EVj.png)

---

#### CPU (after)
![](https://i.imgur.com/cSkD2op.png)

---

#### Improvement Effect

- Monitoring accuracy 🚨 |

---

## Next Action

---

### Publish New Orchestration Tool
- Terratest in Github Actions (AWS/Azure) |
- Daily Integration Test |
- Create new documents |
- Pre Release Check |
- Make Repository to public |

---

### Kubernetes

---

![](https://i.imgur.com/E6u0cYl.jpg)

---

- New apps
- Scalar DL
- Etc

---

### Coming soon...

---

## Finally

---

### I'll ...

---

### Contiune to improvement! 🚧

---

### Keep growing! 🌳

---

### Keep evolving! 🦍
 

---

### Thank for your continued support! 🙇

---

## End

---
