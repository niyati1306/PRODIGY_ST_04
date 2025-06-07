# PRODIGY_ST_04

## **1. Test Overview**
- **Web Page URL:** [https://shoplane-by-lassie.netlify.app/](https://shoplane-by-lassie.netlify.app/)
- **Date of Testing:** 5th February
- **Browsers Tested:** Chrome, Firefox, Safari, Edge
- **Devices Tested:** Desktop, Tablet, Mobile
- **Objective:** Identify layout issues, broken links, and functionality discrepancies across different browsers and devices.

---

## **2. Test Environment**
| Browser  | Version        | Device  | OS            |
|----------|----------------|---------|---------------|
| Chrome   | 110.0.5481.178 | Desktop | Windows 11    |
| Firefox  | 111.0          | Mobile  | Android 13    |
| Safari   | 16.3           | Tablet  | iPadOS 17     |
| Edge     | 110.0.1587.57  | Desktop | macOS Sonoma  |

---

## **3. Test Results**

### **3.1 Layout Issues**
| Browser/Device  | Issue               | Screenshot      | Recommended Fix |
|-----------------|---------------------|-----------------|-----------------|
| Safari (Mobile) | Navbar text overlaps | 📸 [Insert Screenshot] | Use `flex-wrap` in CSS for responsive menus |
| Firefox (Desktop) | Misaligned buttons  | 📸 [Insert Screenshot] | Ensure `display: flex; align-items: center;` |
| All Devices      | Cart logo not visible | 📸 [Insert Screenshot] | Ensure logo is properly loaded and visible, check `z-index` or image path |

---

### **3.2 Broken Links**
| URL                          | Browser | Status        | Recommended Fix            |
|------------------------------|---------|---------------|----------------------------|
| `/about.html`                | Edge    | 404 Not Found | Fix link or update URL     |
| `/contact.html`              | Chrome  | Redirect loop | Check server redirect settings |
| `/clothing-accessories.html` | Chrome  | 404 Not Found | Fix link or update URL     |
| `/clothing-accessories.html` | Firefox | 404 Not Found | Fix link or update URL     |
| `/clothing-accessories.html` | Edge    | 404 Not Found | Fix link or update URL     |

---

### **3.3 Functionality Issues**
| Browser/Device  | Issue                     |  Recommended Fix             |
|-----------------|---------------------------|------------------------------|
| Edge (Desktop)  | Submit button unresponsive | Debug JavaScript errors    |
| Safari (Mobile) | Dropdown menu not working | Ensure `touchstart` event handling |
| All Devices     | Search button doesn't work | Debug the search input functionality, check for JavaScript or API errors |
| All Devices     | No option for adding address/contact | Implement an address/contact section or form |

---

## **4. Summary of Findings**
- **Critical Issues:** Cart logo not visible, submit button unresponsive, dropdown menu not working, broken links for "Clothing and Accessories," search button not functioning, no option to add address/contact.
- **Minor UI Fixes:** Misaligned buttons, navbar text overlap.

---

## **5. Recommendations**
1. **Ensure Responsive Design:**  
   - Use `@media` queries to fix overlapping elements.  
   - Test different screen sizes for better mobile usability.  

2. **Fix Broken Links:**  
   - Verify internal and external links, especially for the "Clothing and Accessories" section.  
   - Implement proper redirects if necessary.  

3. **JavaScript Debugging:**  
   - Check console logs for errors, especially related to the search functionality, submit button, and address/contact section.  
   - Ensure event listeners work correctly across browsers and test with developer tools.  

4. **Add Address/Contact Option:**  
   - Implement a section or form for users to add their address/contact information.  
   - Ensure this functionality is visible and accessible across all devices.  

5. **Use Cross-Browser Testing Tools:**  
   - Utilize **BrowserStack** or **LambdaTest** for wider testing coverage.  
   - Regularly test on real devices for accurate results.  

---
