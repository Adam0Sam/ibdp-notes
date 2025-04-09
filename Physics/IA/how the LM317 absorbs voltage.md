1. **Voltage Distribution:**
    
    - The LED operates at its fixed VfVf​ (e.g., 2V).
        
    - The LM317 "absorbs" the remaining voltage:
        
        Vdrop,LM317=Vin−Vf−1.25 VVdrop,LM317​=Vin​−Vf​−1.25V
        
        For Vin=5VVin​=5V and Vf=2VVf​=2V:
        
        Vdrop,LM317=5V−2V−1.25V=1.75VVdrop,LM317​=5V−2V−1.25V=1.75V
    - The LM317 dynamically adjusts its voltage drop to maintain the desired current, even as RsetRset​ changes.