## 🧩 Flow Diagram – AI Request Router

<!-- This diagram illustrates the flow of how AI requests are routed through the system. 
It shows the decision-making process, including keyword matching, AI classification, 
and escalation paths, to ensure requests are handled appropriately. -->

```mermaid
flowchart TD
    A[New Request Submitted] --> B[Check for Category Keywords]
    B -- Match Found --> C[Route to Appropriate Team]
    B -- No Match --> D[Send to AI Classifier]
    D --> E{Is Confidence High?}
    E -- Yes --> C
    E -- No  --> F[Send to Ops Escalation Queue]
    C --> G[Send Confirmation Email]
    C --> H[Log Request in SharePoint/Excel]
    F --> G
    F --> H

https://mermaid.live/edit#pako:eNpVkU1zmzAQhv_Kzp6dxCY2uByaSTCOM23TNs4lgRxUWEBTkKg-xnY8_u8V4Hgcndid59lXrPaYyZwwxFQUtdxkFVMGnhepAHduk0fawBP9s6QNrO2fhhtD-RtcXHyFuySqKPsLhVQQMUOlVDv4RruNVLl-GwbcORJ-MJNVsJRW5L0YJU_SGgIj4bZtlWwVdzo8E2vOtUd5NDtnkazJ6Z3yAFHNtOYFJ3XkFz0T7x80RFIUPCeREax4Wd0cBiLuJr6QHi5w1nMpfW95CvjZaoh1xmpmuBTw25KlY07Uo_cD2iepZqDihvH6E7VKvsvytDsuYO1WS78kF-Yq3mb0QS-HmefFKhU4wlLxHEOjLI2wIRfUlbjvwBRNRQ2lGLrPnApma5O6Fzw4rWXiVcrmw1TSlhWGBau1q2ybu1UvOCsVa05d5X6HVOQeyGDoef0MDPe4ddV0fDmdXE-Cycz3gsD3R7jD0DX9eTANvszmvnftzT3_MML3PnV8OQ9m47MzOfwH-zO4pA

