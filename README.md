# secure-cloud-config-regulatory-compliance

***LAB Precursor:***

It is important to highlight that during the initial deployment, all resources were exposed directly to the internet. 
Specifically, the Virtual Machines had their Network Security Groups and built-in firewalls configured in an open manner, allowing broad access.  
At this point in the lab, I have hardened the Network Security Groups.

***High-Level Overview:***

+ Inspect MDC Secure Score
+ Inspect MDC Recommendations
+ ENABLE MDC Regulatory Compliance (this takes  a while to appear)
  + NIST 800-53 Compare NIST site with MDC recommendations
 


***Step 1: Inspect MDC Secure Score in Microsoft Defender***

![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/dd8f53ff-143f-4386-997c-ae669a63daad)
![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/af97a68b-f94d-4362-82b4-ba7d6cea7a4c)

In Recommendations - it'll show you all the things contributing to your security score, it'll show you areas that have gaps that you can implement things in Azure or some kind of configuration to make your secure score go up.
You can investigate and get a good sense of how secure your network is.

![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/4bbfbced-3867-497d-83b7-c7b81aa10551)
![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/df5a4611-8d7b-48ca-955c-5f02b224e2c8)

***Step 2: Inspect and Review NIST 800-53 catalogue for MDC Recommendations***

NIST 800-53, crafted by the National Institute of Standards and Technology, stands as a pivotal cybersecurity framework.  
Tailored for federal agencies and organizations, it furnishes a comprehensive set of controls categorized into families, spanning critical domains like access control, risk management, and incident response.   
This framework serves as a linchpin, offering structured guidance to fortify information systems.   
Its significance lies in providing a systematic and nuanced approach to security, shaping the landscape of compliance standards and risk mitigation strategies in diverse technological contexts.  

![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/55789274-8721-4b40-a7bc-558a4bd96005)

Inside of them, there are lots of Subcontrols:

![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/43dfa050-7140-49af-bdab-20bbab9f71d5)

***Step 3: Enable MDC Regulatory Compliance in Microsoft Defender***

![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/f91db9cf-0286-4b29-8cf3-02fc2719e28e)
![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/7383d05f-99ed-463b-8358-b4fe8a8e7a11)
![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/5accba9f-ed57-4b48-96cf-732dbafc7ceb)

Configure NIST 800-53 Rev 5:

![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/6b0602b9-a0e2-48ae-8d4f-dffefeeece3e)
![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/f08d4253-79c3-4dfa-8759-0d1c0872593c)
![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/c57f8f92-8632-4626-a007-81bc72b3719f)

Now select review and create. It will take some time to appear so be patient.

***Step 5: Check Microsoft Defender for Cloud | Regulatory Compliance***

![image](https://github.com/hoanghuydang/secure-cloud-config-regulatory-compliance/assets/127445164/29735da6-da50-4a38-8b60-dfd00851487c)

SUCCESS it has appeared.

***Lab Fin***
