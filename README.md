### **EduChain BUIDL Submission**

#### **Profile**  
- **BUIDL Name**: EduChain  
- **Vision**:  
  > "To create an uncensorable education verification system that works in internet blackouts, turning refugee voices into blockchain-anchored credentials using offline AI and mesh networking."  
- **Category**: **Al - Decentralized Intelligence**  

#### **Links**  
| Type | URL |
|------|-----|
| **GitHub** | `(https://github.com/Shivavigneshkannan-k/EDUCHAIN)` |


### **Details**  
#### **Problem Solved**  
260M+ children lack education access. Refugees can't prove skills due to:  
- No internet in crisis zones  
- Paper records destroyed in conflicts  
- Centralized systems exclude the disconnected  

#### **Solution**  
EduChain enables **offline credential minting** via:  
1. **Voice-First Interface**  
   - Whisper.cpp on-device speech-to-text  
   - Works on $50 Android phones  
2. **Bluetooth Mesh Network**  
   - Propagates credentials teacher-to-teacher  
   - Solar-powered mesh nodes extend range  
3. **ICP Blockchain Anchoring**  
   - Batch-mint NFTs when internet available  
   - Zero gas fees via reverse gas model  

#### **Tech Stack**  
```mermaid
graph TD
    subgraph Student Device
        A[Voice Recording] --> B[On-Device Whisper.cpp]
        B --> C[Validation Engine]
        C --> D[Create Credential]
        D --> E[SQLite Storage]
        E --> F[Bluetooth LE Broadcast]
        style A fill:#4CAF50,stroke:#2E7D32
        style B fill:#81C784,stroke:#2E7D32
    end




    subgraph Bluetooth Mesh Network
        F --> G{Mesh Routing}
        G -->|Teacher Nearby| H[Teacher Device]
        G -->|No Teacher| I[P2P Forwarding]
        I --> J[Mesh Node]
        J -->|Store & Forward| H
        style G fill:#FFC107,stroke:#FFA000
    end




    subgraph Teacher Device
        H --> K[Pending Credentials]
        K --> L[Review Interface]
        L --> M{Decision}
        M -->|Approve| N[Update Status]
        M -->|Reject| O[Mark Rejected]
        N --> P[BLE Broadcast]
        O --> P[BLE Broadcast]
        style L fill:#2196F3,stroke:#0D47A1
    end




    subgraph Blockchain Sync
        P --> Q{Internet?}
        Q -->|Available| R[Batch to ICP]
        Q -->|Unavailable| S[Local Storage]
        S -->|Later Sync| R
        R --> T[Mint NFT]
        T --> U[Store on IPFS]
        style R fill:#9C27B0,stroke:#6A1B9A
    end




    subgraph Verification
        U --> V[Employer Portal]
        V --> W[Verify Credential]
        W --> X[Skill Validation]
        style V fill:#F44336,stroke:#C62828
    end




    A -->|Offline First| B
    F -->|BLE/ WiFi Direct| G
    P -->|Approved Creds| Q
    U -->|CID Reference| V
```

#### **Key Innovations**  
- ✅ **Offline-First Design**: Full functionality without internet  
- ✅ **Refugee Camp Mode**: Ultra-low bandwidth (<1KB/credential)  
- ✅ **Censorship Resistance**: Credentials survive via mesh persistence  

---

### **Team**  
| Name | Role | Expertise |
|------|------|-----------|
| Jasom santo leon J | BE CSE student | Full-Stack, ICP, React Native |
| Shiva vignesh kannan | AI/Blockchain | Whisper.cpp, Cryptography |
| kavi | UX/Testing | Refugee camp deployments |  
| gayathri | Full-Stack, ICP, React Native |
| gayathri | Full-Stack, ICP, React Native |

*Add LinkedIn/GitHub links for each member*

---

### **Contact**  
- **Email**: jasonsantoleonj.cse2023@citchennai.net  

### **Submission**  
#### **Progress**  
- [x] Voice-to-credential MVP  
- [ ] Bluetooth mesh prototype  
- [ ] ICP canister integration (in progress)  
- [ ] Field testing in simulated environments  

#### **Requested Support**  
- Technical guidance from DFINITY engineers  
- Access to ICP HUBS network  
- Grant interviews for scaling  
