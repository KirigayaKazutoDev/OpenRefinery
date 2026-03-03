# **OpenRefinery**

# **TECHNICAL SPECIFICATION: HYBRID PLASTIC-TO-FUEL SYSTEM**

## **Author: Gemini AI & Kazuto Kirigaya**

## **Subject: Waste-to-Energy (WTE) Conversion and Automated Multi-Stage Fuel Refinement**

### **1\. ABSTRACT**

This paper outlines the theoretical and practical design of a decentralized, hybrid refinery capable of converting post-consumer plastic waste into high-quality liquid fuels. The system utilizes a Blest-style induction reactor for primary decomposition, followed by a multi-stage refinement process involving fractional distillation, density-based mechanical separation, and advanced electrolytic dehydration to ensure engine-grade purity.

### **2\. CORE PROCESS: THERMAL DECOMPOSITION (PYROLYSIS)**

The fundamental principle is the "cracking" of long-chain hydrocarbons (polymers) into shorter chains (C5-C40) in the absence of oxygen.

#### **2.1 Atmospheric Control**

To prevent combustion and explosion, the reactor must be void of Oxygen (![][image1]).

* **Method:** ![][image2] Displacement (Purging).  
* **Execution:** ![][image2] is injected at the reactor base. Due to its higher density compared to air, it displaces ![][image1] through the top exhaust. A "Bubbler" (water-lock) at the end of the line prevents atmospheric backflow.

#### **2.2 Thermal Core (Blest Integration)**

The system is designed to utilize or emulate a **Blest-style induction reactor**.

* **Induction Heating:** Rapid, efficient melting of plastic waste.  
* **Thermal Profile:** Maintained between 350°C and 500°C.  
* **Catalyst:** Using Zeolite (Y-Zeolite) lowers the required activation energy and increases the octane rating of the resulting gasoline.

### **3\. FRACTIONAL DISTILLATION AND CONDENSATION**

Post-reactor vapors contain a mixture of gas, gasoline, kerosene, and diesel.

#### **3.1 The Three-Stage Condenser Array**

To achieve tank-ready separation, the vapor stream is passed through three temperature-controlled zones:

1. **Tank 1 (Diesel):** Maintained at \~200°C. Heavy chains condense here.  
2. **Tank 2 (Kerosene):** Maintained at \~120°C. Intermediate chains condense.  
3. **Tank 3 (Gasoline):** Maintained at \~15°C via ice-water or active refrigeration.

### **4\. ADVANCED SEPARATION: MECHANICAL & CHEMICAL DEHYDRATION**

#### **4.1 Phase I: The Density Float (Dichteschwimmer)**

Water settles at the bottom due to density (![][image3]).

* **Logic:** A spherical float calibrated to ![][image4] sinks in gasoline (sealing the drain) but rises in water (opening the drain). This removes the bulk of the aqueous contaminants mechanically.

#### **4.2 Phase II: Electrolytic Moisture Elimination (Ultra-Purity)**

To remove the final 1% of emulsified water, the system activates an electrolytic cell at the bottom of the gasoline chamber.

* **Electrode Design:** \- **Bottom:** A solid metal plate (Pure Plate).  
  * **Top:** A **Grid-like Mesh Electrode** suspended slightly above the plate. This allows ![][image5] and ![][image1] gas bubbles to rise freely through the fuel layer without being trapped.  
* **Safety Interlock:** Before activation, an electronic solenoid valve **closes** the path to the main storage tank to isolate the reaction.  
* **Gas Extraction:** ![][image5] and ![][image1] are routed through a dedicated gas exhaust pipe, which is electronically opened during the process.

### **5\. PURIFICATION AND SYSTEM PROTECTION**

1. **Demister Pad:** A stainless steel mesh at the reactor exit to catch liquid aerosols (wax) before they reach the condenser.  
2. **Active Adsorption:** Final filtration through Activated Carbon/Silica Gel.  
3. **Corrosion Shielding:** A high-velocity cooling fan is located beneath the water chamber. A **mechanical shutter** protects the fan from moisture/corrosion. The shutter opens and the fan activates only *after* sensors confirm that all water has been electrolyzed and converted to gas.

### **6\. MATHEMATICAL FOUNDATION (BUOYANCY)**

The float design is governed by Archimedes' Principle:

![][image6]For the float to operate correctly:

### **![][image7]7\. CONCLUSION**

By integrating ![][image2] purging, fractional condensation, mechanical buoyancy separation, and high-frequency electrolytic dehydration, the OpenRefinery achieves a near-perfect energy recovery cycle. This hybrid approach transforms waste into a high-energy asset, pushing the boundaries of decentralized energy production.

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABcAAAAZCAYAAADaILXQAAABvklEQVR4Xu2Uu0sDQRDGL4hgofiAAzW5XF4SrQ8VrMTCxsYmhYX+CWppJ9jYCRJSiSCCIIKIYGMjVqJNSqtoZ6miWAb0N+YubiaJedhJPvhgd76Z2dnZh2V10Co8z+uOxWLDjuOMptPpPq23ixBJZ13XfYEP8BF+wFvt2BKSyaRD4nNJyrQrsEcikSFsp9FoNGO4N4d4PD5F8BO8J3lM6wHQP2FW238FAdewSGUrWjMhyfG5g4Naqwu/ohuKHtCaCd+vIIestZqgioRf0arWNFpNHsL5qJmtplIp2y/igGlI61WQ+0vAlSxgNQjg0OflXGjdYmBjoU1se9jWE4lEv+lvJj+sEKohO8y5xrmQ2CNhlPm4W7oQ+XA4HClHIPRgvGiUnB5P4vMs1Qc25tmg94xn4Bv5Nn6irO8KtmUBWahC8CG7w+dSWmIZrWO+AydkLIswLtQqUrYsd/zYtu3ewCg9FGf4irZmGS9WQb6LXbfeA5Rr6Jb+koLsBC4zfocnclW1vwn0DH55vogxrZXh939OEjNeauYnxG+amDM4orU/g6Q5+dRkLDeF+Zb2aQsk2ndLLzZgES5ovw7+Cb4ABvFwwOB9wUcAAAAASUVORK5CYII=>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACYAAAAZCAYAAABdEVzWAAACrUlEQVR4Xu2Wu2uTURjGE4KgqHgNqUmT70sU4gUVCZrBycW1xUFFdHAQcXGt6NbN/gVCiUNBdBCLoigIxctSEURU1IKCCGpBKzgIFQv6e5pz9O3xS9o66NA88HBy3st5L+fyJZXqYIEgnc/n1xaLxXy1Wl3uhbVabVEul1tqDZMgv3K5nONnJtT9LdJRFF2HX+F3+AZ+geXu7u4ljI1SqXQkdBIqlcoK9APwA3ztxs9xHJ8NbecFFlkHr7DQVardlvpdbQb5QxK6xfgR7rB+ArrDyD/BQXXLidOs1YtsgnGltZ8TSGIXzu/gOAF2h3qBheuqHjasXFuLzznYxzRtdR4kuh6/99hsDnVtgdMo/AFPp1ovnkf/KtxGEj6IfLJQKKyxcgudUa0f+s4Kl9Rjd1gT4RIbtVVzpkrIXsApaxvCJ0YRp0JdSxCo4qo5GeoslBg2+3UBvAy/flfUU2sbgoS65p0YDkMEfABXhbp2MGdu1i3C9gR2ExS3M9QlwrV4BF5ItThbrUCwHtctPQf1UO+BbnHUfH5G7HvIfBMc1G22uzANk9jQDEUCWOCS3ik/N4m17QRBt2IzDg95mfMdcF0fgzds0tNXHeHluSSGTb+dc1H2Iptsl5hbv6ECfFfUQXgN2UXNlTD8hqx3hrMOPYqbf7TTAH1ZN9DK9Dbh+1bJKUmr81CwqPkFeW5k2tph+EhzFaXi4qSL4ZzHCLDdygm8Bd7F6YCVeyCPFVQLByp91vRg31dRge4X1AzXvdtx0pcBxR74Ek7BZ/A8hk/gPbgxtLdQYHgHDlPEMcYzWks3VVsZ2ltg06ekSHB1qLPI6PHUW0UyPbArNGgDdWgfPkc1EmhDaJAEbBvZbHZZKP+v0PfZXIg6PB7a/FPov5y2L2o+NZ6J/1g66GDB4Scpmb727teKqAAAAABJRU5ErkJggg==>

[image3]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFEAAAAYCAYAAACC2BGSAAAD8klEQVR4Xu1YTUhUURQeiSCDIPshyXHem8kQgoiSCBKCINtEaWDR7yYIMWhVkLgoskULKYSSiJAi0OiHFglJ9rNqUVCkBVGEQwvJoERUJKEB+z7fuXbnzDgzmm/Smg8+3rvnnHfvO9+997w7EwjkkBbBYDA/FAodchznHO5Xa38OaVBWVjbfdd0miLgHIh4EB9Cu0nE5pICIWAMRK8A1EPEL2KDjcsgQEPE0BOyCqK72zUkgjzpt8xNSEz9g3E3aNyeBRBYjoXZt9xv8qGDcHvAkmnnamQ9HI/gKjIFjcQEpwKWN+PfoYwnbmLFytPtYS3TsDCEP/Tdj2Frt8AMYZx/GG0VeR0tLSxfh/hn4DVwfF4iAAhFxN/g8UxEpFGJbwF7bjvYR9Flt22YKSKoQ7CwuLl6lfX6Ak4V8hnCtpE7gSwpJQXXsOCylMxLR+lo9tu1IcCNs9/xYjUimCn23+dF3MkjpuAleQr7X0X7LvHXcBKYh4mHGchDbXlRUFIQtyqtt/1PIym+jkNrnM1hCwiLePO2Mw1RFlBlKEBErcSXt3AK23Qb8F8ABvNgpxO9yvLrzyPFKylcdT8jWag6ooi6r5S6uNZw49FOB9vdwOLwC3I77z+BP2I/j2gGeAHc4Xv1vCHkH6ae47sX1I8d3p/sVzrKIMbz0edOWWhNlrZssAdgfUBTbJqvzGjhqxVVyfJYVY+NYsPXafaP9ic+BDzkREmd2V4uJmxKyKCK3xxhf2BjMuCmeYUyHSdaybQYHwW5jk5XZYNdN2Oow3o2AtYplzJhrlQczAfQZ25SQRRH5LP0TxxQzbppnEn5uyQrjO7Rqnw2KSNo2GbPfXrHyUeynz47NGNMQkbWFCSQTMfEsZQG+1+AQRUBy+/niuN+p4wy4jXme1XaOnewdNGatiFK0WVOSHXG6S0pKltt2G/DfkvpXC/Gu4IOwVMdYGD9gayPB50XElEnPChFdr860gm/ADWIrxP07CmbHirgXbZsG/C/SCDcBjgN2ajuBCYigryg4qFwU/oBpZEPEPG5BJL8OD3dRRLZJDLyAAc7vIwHr1lXzINrHwBHTlq/lnXR/XjJpsM/xfov2oM/bEORMJBIJ6VhXDtjabiBHlBEwbNnKOfF8f8mjieQ9sBBc5ng/c4dhr+RxSCaLH5Zh+tBHgT2O73C9bdWIgbel+zXB5BD7hC9ubCL+Vsc7p0WNXbZ8JxM0tslAYShS1pP/G+B254xrOwEBqiFizLRlchIO2P89pO7UBxKFYR2rd+QXi/y7dB+ib1FxOQQ8sfqxys6abcorbJfBH473fx1FXIv7dm7/+MdzyAgs/hCwjUJqXw7/IH4BkT5gePtZbdUAAAAASUVORK5CYII=>

[image4]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFsAAAAYCAYAAACV+oFbAAAFI0lEQVR4Xu2Za2hcRRTHNwRB8UFVQqpJ9u4mwaiI2AYNFtSCVSxBUnxRC0opihShIIoP8INWRKgiShGLpShFqcVAfWGE0tCKiIpKtGANtan0QytKA00t9EOg/v6ZM+nZ8WYb624+mP3Dn7nnzJnXmXPPzN0tFBqoFZqLxeKd8M2Ojo7rkZtSgwZqg6Ysy56Aj/PcTPmn5NSogdpAzr6LqH7Ann+E23p7e89JDRuoLeTsg+Vy+Ya04n8NFr0q1dUT5OqbGPN7IvyewnzK2aVS6Vy4PdXPBXD4Vzh800xpRKH/B5Nboef29vZLkH9oa2trTw1TYLcI7qPzBwvhcLgbHqav1dGmp6fnQnTD8JQnNgtO91RbMJ91jLE+1dcDjHMjPApfNXkrnIT9qa3C/xoqNhRc6CP/Dl/0uhTaOWy2wTVeL8ejG41yjrN/wdErfZtagmA5jzEG4ZK0rh4gP9/OWH+xpsck29j7Ojs7i6mtXrmn4YDXmXP2ol/o9R5s0uXY/Jq21T0T/YEoy9lswIfepp7Q+BpP46Z19YAF3Qa4FV/cTznG+MtSu6ncRuWnlH1eLx08zq7d7PUe0dnwk5aWlguiXm2kj/JcO5ux1yuAUn29ocBU4M2Uq6cdZl8909AuZSGvVp00TrwXuxOyha9g/xHlZyWXj6Oz0X1BeYj6cZ4/9v3kwV7PI9hup9192vwsnPa3UY7BLWkbdEvgoFJJUtVEP6up20y/PTxfx/MofXUit1LuQZ6gfJ/yDfgW7IeT6DZhv5LnXVk4k36De2dzplXAXvmjZ+vsQljECvUhe3gQLvYGMWd3dXV1SNZGIO+kLHm7FNiMsNBv4MUmKxce1R0WXqtASdtg+xJcl+pt407EqIvrztwhxnT6kE/S/smCnVUaPwsO/zwGEPKzWmsxfMTMHv/V2Zo8gz6F7c+yN04oiqJNKVzDnnfNpNMGVf3K0sLhcMy9mov1r8/iXFC3i/lc7XV2YA6pv6jTuPT3iE9/5ov9PmI1PpzUfKNOTtY8zuSbf4ABumh86GycbQfDZrgbXgYfghNqB4+l9h62sMOpYzzkHC02OjuziMqqO3uHNtfrNIbGEr0+hc1pejxBcpYEI/0PaB7VfJOL7u7ui5jMnhxnv2cdVtw0PKjf4l9zpy/DUZu00szryJPeRtFzpv4VebLJwgGuU145VSki9zqKzULqO1O9SxljaZ1H3Z0NmpjgO+mibRD9erXI6z2yEP0Vk/N1ra2t5/s7tk8ZM6UvD+o/YF59triNufdWB2yW56Ul29j9cDyt85gLZ6vDVTRcm+hG4VA81TvCrUWn8XDMaRosC3fKimiKOdLEqc3U2+NtSiFn525UBDY/0e7WVD8DNM7bqdIQ365TevYVft1z4myLvt0ld11DPi6HRDkOYINMvQWUpSwcjO+6g0aLfhjdiGt7C/zWyfE2UnG3T4HNjixcK3XNO6A28AXaXVlInGbRu9PrPOJcKe4oWFvelCsscJp1/bM1fgevUmo0v3yZBV8MmI2+Sx7Ngh9eUxBWjjQL2K1iWTFcnfQ7x6xhJ/tSc8TSvFdZoG4tNi/Dfn8LmAnYHSmHj6roWP32stgcMn242kGtlLb8dOt8yIFykByH2JzWz0so3+O8wbyNK4c780lFm2SlMeShUpWfFhqoAovWr3nNL03r0K+BxzL7oakY7r0bU7sG/gVw4IgcrtSB2EzkLoDPII9n4T++pvjLo6I9bd9AjYGj+9mA51J9A/McfwOTkqx/LXm+qAAAAABJRU5ErkJggg==>

[image5]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAZCAYAAAArK+5dAAABuklEQVR4Xu2UzytEURTHZ5KiCIuXxfy4M/OmJpYmETvFRmKBWLD3H1jYTpKlpUjKgjUrNQtK2YiylIVkNyPZjFJ8jnffeHMaejUWkm99e3PO997vOffXRCL/+FVIpVKDcN8Ys6lYSCaTXWhrdTRhn/aqi1gsFsdoFqNlJr3CDYnhcD6fb+Y7ChfJX8NTxs0TTziO06a9voUYw0MMWrSWTqfH0CoY92otFHK5XDsGRVmF1gRoK/BNxmktFKQzDB6kU63JimRlUkBroUGBBTGQ89BaIpFw0e/kfLQWCnJT4LkUsIdbQ/JHosFjPTcU6LCfySVY1pp/Nrb4alCLx+Otxruu67AnqNWAPV6yHV5pzT8bWAmejy28Ta6bbwE+4jMZnOsjismOLbCnRSZNGe9t3AbPx17bezumk99nsPg50yKbzTrSuRSQlWjdeG9Dite8D+IR+ById+GNH1dhvP0Tg0vXdRNKbiL/BF9Y5TRxVOkfsKspMWammqSbAZJla16l7Hkmk+lAP9GaMODr+6TIX/CZi3zRQEPA/KDe4/wRyB8hBYZsGOV3oWZAI8Bs3Hi3K7iFW3rcP/4w3gGRdovN3d/3dAAAAABJRU5ErkJggg==>

[image6]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAmwAAAA9CAYAAAAQ2DVeAAAEjElEQVR4Xu3dPYgcZRgH8D2CoOJnIcrlbmf3EokIFuaQiIKChSAqigS7WAgi2lgIRkWwiGJhmcJChCgcgpWChVGJioLa+YWgxmAhIRAUVAIpAvF53Jn48uZyudvbHHfH7wcvO/PMu/Ox1Z/3nZnt9QAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABgU5vq9/u3R3t4qVZ/aaOor61pmrvm5+cvKrbfX2x7qPwuAMC6MDc3d2WElXcjrJyIdjrakWi/ti2Xs3a6/t5G0V7bb+11nBgMBm9Gu7jbHss/R/1UtL+jfV5+FwBgXYmw8stiwWx2dnZbhJrv6vpG0wa2Q3U9At3uqH9U1wEA1p0ILf9EO1rXI7BNb4aRpzawfbtI/YsIpHfWdQCAdSXv6WoDzf6u1u/3D27fvv2acFnUbyv7r6U4j8fi+K/n1G29bSXa6/ujrEVQuzVqw7K2Sltif6/GOb+Yy9PT05fWHQAAxrJ169aZDDQRNPa0pQweC/E5VfZbY1vifJ6K89g3HA7viM8fI2AN6k7LlWEt2slufceOHZfH/j8o+6xGnNoNsf+vYp/3xfLjsXw42k91PwCAsUTAeDbCxQ8RNh7J0BbLH0dtV9mnfLLyXPJm/pxCPV+LAHZt/d1aM3oI4uViPQPQ4bJPypG3OO4Ddb2W4SlDabH+ZVzrfNnnXPIYMzMz19f1Toa/DIPR7ulqeaymGLEEABhbhqwIFu9He6OrRai6JadDczk/Y9snEW4O9NZoxC3C0SVxzGPxeVNXi/XjiwW2qL2d4SjOb67eVoo+h7rA1k4BP99bxvW0ffMYR851jHxwIdrX0a7uau057S77AQCMZTgc3h3h4mSEixu7Woa4sk8GuGxlbTGTGmGL/TwR5/NKWcsAlMGprKUVjLDtz31E30F8flpvX0p7jEFdTxFor4hz/awMZ/lbZi23lX0BAMYS4eWFdjTozOhQLbbt6UbclhL7ean5/x1uS7Wl7u3KF/keiD73doU8t1g/keGy7LgSg9G0b17na7n/evu48txydK0MtPl7NaZDAYDVyqm+CDHXRbD4PYNMjnzlet2vCyTZP+/VytGvus8kxf53xfn8Gcfc22v/hSHWj0X9qrrvSrQPLuSrS56st61WnNuDsd9HY3Eqlt9rg+GZEUsAgLFEqHgrg0XV/lqk381Ne+9YTvHF8r66zyRlIGwDz8FmdN/Z0Vh+pu63Uu11HM/QWW+bgKlmFHxP9UdPth4zHQoArJl2eu+/F87Ozs5ui+Wn6z6TFPtfyOATi1vyXrflPJ26HO3o4HN1fdLa3+usf4wAALhg2hGvhZySjPZhbxlPVq5GM3pf2ll/IbVeNaO/9Drzfrdm9L+l35R9AAAuqLy3rRm99uOdSUxNnk+OTvWrJ0TXswxr0b7vjaZFdzajhyp21v0AADaN1T5cAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABvPv+22B8NQ1B+1AAAAAElFTkSuQmCC>

[image7]: <data:image/png;base64,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>
