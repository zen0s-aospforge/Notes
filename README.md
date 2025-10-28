### **Manual DC Dimming Control via Termux**

**⚙️ Path:**

```
/sys/devices/platform/soc/soc:qcom,dsi-display-primary/dimlayer_exposure
```

**📋 Requirements:**

* Root access
* Termux with `su` binary (Magisk, etc.)

---

### **🟢 Enable DC Dimming**

```bash
su -c "echo 1 > /sys/devices/platform/soc/soc:qcom,dsi-display-primary/dimlayer_exposure"
```

### **🔴 Disable DC Dimming**

```bash
su -c "echo 0 > /sys/devices/platform/soc/soc:qcom,dsi-display-primary/dimlayer_exposure"
```

### **⚙️ Check Current Value**

```bash
su -c "cat /sys/devices/platform/soc/soc:qcom,dsi-display-primary/dimlayer_exposure"
```

---
