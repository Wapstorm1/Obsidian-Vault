## **🧪 How to Test Them:**

  

### **✅ 1.** 

### **Switch Between Apps**

- Open app → press Home → open another app → return
    
- Look for:
    
    - Data loss?
        
    - Crashes?
        
    - Session timeouts?
        
    

---

### **✅ 2.** 

### **Kill the App**

- Swipe up from app switcher or use ADB (adb shell am force-stop) or Xcode tools
    
- Then relaunch
    
- Expectation: clean restart without crash or corruption
    

---

### **✅ 3.** 

### **Interruptions**

- While using app:
    
    - Get a phone call
        
    - Receive a push notification
        
    - Plug/unplug charger
        
    
- Check how app behaves — freezes? reloads?
    

---

### **✅ 4.** 

### **Lock/Unlock the Screen**

- Use power button
    
- Leave locked for 1–2 mins
    
- Unlock and observe: does the app recover state correctly?
    

---

### **✅ 5.** 

### **Cold vs Warm Launch**

- Cold = app fully closed before opening
    
- Warm = app already in memory
    
- Compare launch times, splash screens, and stored state
    

---

### **✅ 6.** 

### **Low Battery, Low Memory Scenarios**

- Simulate using emulators or background-heavy apps
    
- Observe how the app handles being force-killed