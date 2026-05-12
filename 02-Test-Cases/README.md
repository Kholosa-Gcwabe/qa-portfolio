# Test Cases

## TC_POS_001: Login
| Field | Details |
|-------|---------|
| **Title** | Verify user can log in |
| **Precondition** | App is open |
| **Steps** | 1. Enter username&lt;br&gt;2. Enter password&lt;br&gt;3. Select role&lt;br&gt;4. Click "Sign In" |
| **Expected** | User sees the dashboard |
| **Actual** | User reached dashboard |
| **Status** | Pass |

*(No screenshot available for this test case)*

---

## TC_POS_002: Select One Item
| Field | Details |
|-------|---------|
| **Title** | Add "Pap (R20)" to order |
| **Precondition** | User is logged in |
| **Steps** | 1. Click "Pap (R20)" |
| **Expected** | Item appears in receipt, total shows R23.00 (with VAT) |
| **Actual** | Item added. Subtotal R20.00, VAT R3.00, Total R23.00. Message: "Added Pap" |
| **Status** | Pass |

**Screenshot:**
![TC_POS_002 - Pap added to order](https://github.com/kholosa-gcwabe/qa-portfolio/blob/main/03-Test-Execution/TC_POS_002.png?raw=true)

---

## TC_POS_003: Select Multiple Items
| Field | Details |
|-------|---------|
| **Title** | Add two different items |
| **Precondition** | User is on dashboard |
| **Steps** | 1. Click "Pap (R20)"&lt;br&gt;2. Click "Chakalaka (R25)" |
| **Expected** | Both items in receipt, total R51.75 |
| **Actual** | Both added. Subtotal R45.00, VAT R6.75, Total R51.75 |
| **Status** | Pass |

**Screenshot:**
![TC_POS_003 - Multiple items in order](https://github.com/kholosa-gcwabe/qa-portfolio/blob/main/03-Test-Execution/TC_POS_003.png?raw=true)

---

## TC_POS_004: Add Same Item Multiple Times
| Field | Details |
|-------|---------|
| **Title** | Click "Pap" three times |
| **Precondition** | Dashboard is loaded |
| **Steps** | 1. Click "Pap (R20)" three times |
| **Expected** | Item appears 3 times, total R69.00 |
| **Actual** | Item listed 3 times. Subtotal R60.00, VAT R9.00, Total R69.00 |
| **Status** | Pass |
| **Note** | Suggestion: Show "Pap x3" instead of 3 separate lines |

**Screenshot:**
![TC_POS_004 - Repeated items displayed](https://github.com/kholosa-gcwabe/qa-portfolio/blob/main/03-Test-Execution/TC_POS_004.png?raw=true)

---

## TC_POS_005: Clear Order
| Field | Details |
|-------|---------|
| **Title** | Remove all items from order |
| **Precondition** | Order has items |
| **Steps** | 1. Click "Clear All" |
| **Expected** | Confirmation popup appears, then all items removed, total resets to R0.00 |
| **Actual** | Popup asked "Clear current order?" Clicked OK. All items removed. Total R0.00 |
| **Status** | Pass |

**Screenshot:**
![TC_POS_005 - Clear order confirmation popup](https://github.com/kholosa-gcwabe/qa-portfolio/blob/main/03-Test-Execution/TC_POS_005.png?raw=true)

---

## TC_POS_006: Confirm Order
| Field | Details |
|-------|---------|
| **Title** | Complete and process order |
| **Precondition** | Items are selected |
| **Steps** | 1. Click "Confirm Order" |
| **Expected** | Order processed, receipt clears, system ready for next order |
| **Actual** | Message: "Order #2 confirmed!" Receipt cleared. Totals reset to R0.00 |
| **Status** | Pass |
| **Note** | Suggestion: Show timestamp or receipt summary after confirmation |

**Screenshot:**
![TC_POS_006 - Order confirmed message](https://github.com/kholosa-gcwabe/qa-portfolio/blob/main/03-Test-Execution/TC_POS_006.png?raw=true)
