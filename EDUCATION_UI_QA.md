# ROOTED Education — UI Front-End QA Requirements

This document governs Education UI correctness.

Backend authority ALWAYS wins.

---

## 1. Navigation & Routing

- Institution tools visible only to institutions  
- Vendor bid tools only for Premium+  
- Kids Mode UI fully isolated  

---

## 2. RFQ UI

### Required:
- Clear multi-step creation flow  
- Explanation of what RFQs are  
- File attachments (optional future)  
- Clear distinction between:
  - Open RFQs  
  - Closed RFQs  
  - Awarded RFQs  

### Forbidden:
- Showing bids to non-Premium+ vendors  
- Showing pricing in Kids Mode  

---

## 3. Bid UI

- Comparison views must be clean & simple  
- No sorting by non-governed metrics  
- No “recommended vendor” bias  
- Must obey:
  - Tier gates  
  - Specialty rules  
  - Vertical access law  

---

## 4. Discovery UI

- All educational experiences must pass Kids Mode filters  
- Must reflect backend rotation logic  
- Exactly 6–8 results per discovery row  

---

## 5. Kids Mode UI (when activated)

- Remove cost  
- Remove booking buttons  
- Allow only education-friendly surfaces  

---

## 6. Accessibility

- Contrast-safe  
- Extra-large tap targets  
- No hover-only elements  
- Dyslexia-friendly spacing  

---

END OF QA
