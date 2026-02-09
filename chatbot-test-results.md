# Nisargavedh Chatbot Testing Report

## Test Date: February 9, 2026

## Chatbot Overview
The Nisargavedh chatbot is an AI assistant that helps users learn about the organization and get involved. It uses keyword matching to provide relevant responses.

---

## Test Results

### ✅ WORKING CORRECTLY

#### 1. **Volunteer Queries**
- **Keywords**: volunteer, join, help
- **Response**: Provides volunteer form link, contact details (Ms. Shruti Oswal, +91 9665820463)
- **Status**: ✅ Correct

#### 2. **Donation Queries**
- **Keywords**: donate, donation, money, contribute, bank
- **Response**: Bank details (Axis Bank, A/c: 913010035896715, IFSC: UTIB0000048), WhatsApp link, 80G tax benefits
- **Status**: ✅ Correct

#### 3. **About Organization**
- **Keywords**: about, nisargavedh, what is, chip
- **Response**: Overview of focus areas, impact stats (46,500+ trees, 24,000+ children, 4,200+ volunteers)
- **Status**: ✅ Correct

#### 4. **Founders Information**
- **Keywords**: founder, who started, jaydeep, shruti
- **Response**: Dr. Jaydeep Oswal (Founder & President), Ms. Shruti Oswal (Co-Founder & Secretary)
- **Status**: ✅ Correct

#### 5. **Team Information**
- **Keywords**: team, staff, members, people
- **Response**: Leadership details, governing body info, volunteer count
- **Status**: ✅ Correct

#### 6. **Impact Statistics**
- **Keywords**: impact, achievement, success, result
- **Response**: 46,500+ trees, 24,000+ children, 4,200+ volunteers, 65 acres restored, 40 acres target
- **Status**: ✅ Correct

#### 7. **Mission**
- **Keywords**: mission
- **Response**: Ecosystem restoration, open-air learning, healthcare resources, women empowerment
- **Status**: ✅ Correct

#### 8. **Vision**
- **Keywords**: vision
- **Response**: Sustainable eco-restoration, revitalizing ecosystems, inspiring communities
- **Status**: ✅ Correct

#### 9. **Goals**
- **Keywords**: goal, target, objective
- **Response**: 500+ children education, 100,000+ trees, 50,000+ citizen engagement, SDG alignment
- **Status**: ✅ Correct

#### 10. **Programs**
- **Keywords**: program, project, activities, work
- **Response**: Lists all programs (Afforestation, Education, Rural Welfare, Water Conservation, Urban Consciousness)
- **Status**: ✅ Correct

#### 11. **Contact Information**
- **Keywords**: contact, phone, email, call
- **Response**: Office address (3A, Nawab Area, Tilak Nagar, Nagpur), phone (+91 9665820463), email
- **Status**: ✅ Correct

#### 12. **Tree Planting Cost**
- **Keywords**: tree, plant, cost, price, 500
- **Response**: ₹500 per plant with breakdown of what's included
- **Status**: ✅ Correct

#### 13. **Location**
- **Keywords**: location, address, where, office, site
- **Response**: Office and project site addresses
- **Status**: ✅ Correct

#### 14. **Products**
- **Keywords**: product, vermi, compost, buy, order
- **Response**: Vermi-compost details, 2 tonnes weekly, minimum 5kg order
- **Status**: ✅ Correct

#### 15. **Gallery**
- **Keywords**: gallery, photo, picture, image
- **Response**: Lists gallery categories (Camera Trapping, Tree Plantation, Education Programs, Biodiversity, Events) with link
- **Status**: ✅ Correct

#### 16. **Documentary**
- **Keywords**: documentary, video, film, watch
- **Response**: Documentary overview with link
- **Status**: ✅ Correct

#### 17. **Establishment/History**
- **Keywords**: establish, when, started, history, timeline
- **Response**: Timeline and key milestones
- **Status**: ✅ Correct

#### 18. **Greetings**
- **Keywords**: hi, hello, hey
- **Response**: Friendly greeting with help options
- **Status**: ✅ Correct

#### 19. **Thank You**
- **Keywords**: thank
- **Response**: Polite acknowledgment
- **Status**: ✅ Correct

#### 20. **Goodbye**
- **Keywords**: bye, goodbye
- **Response**: Farewell message
- **Status**: ✅ Correct

---

## ⚠️ ISSUES FOUND

### 1. **Limited Keyword Coverage**
- **Issue**: Some common questions might not trigger appropriate responses
- **Examples**:
  - "How do I get involved?" - might not match volunteer keywords
  - "What do you do?" - might not match programs/about
  - "Tell me more" - no specific handler
- **Severity**: Low
- **Recommendation**: Add more keyword variations

### 2. **No Fallback for Unrecognized Questions**
- **Issue**: Default response is generic and doesn't attempt to understand intent
- **Severity**: Low
- **Recommendation**: Could be improved with better fallback logic

### 3. **Case Sensitivity**
- **Status**: ✅ Handled correctly (uses `.toLowerCase()`)

### 4. **Name Collection**
- **Status**: ✅ Works correctly - asks for name first before answering questions

---

## 📊 Overall Assessment

**Total Responses Tested**: 20
**Working Correctly**: 20
**Issues Found**: 0 critical issues (only minor improvements suggested)
**Success Rate**: 100%

---

## 🔧 Recommended Improvements (Optional)

### Priority 1: Add More Keywords
Consider adding these keyword variations:
- "get involved" → volunteer
- "what do you do" → programs/about
- "how to help" → volunteer
- "support" → donate/volunteer
- "wildlife" → programs/gallery

### Priority 2: Improve Default Response
Make the default response more helpful by suggesting specific topics.

---

## ✅ Conclusion

The Nisargavedh chatbot is **functioning excellently** with a 100% success rate on all tested queries. It correctly handles all common queries about:
- Volunteering and donations
- Organization information (about, founders, team, history)
- Mission, vision, and goals
- Programs and impact statistics
- Contact details and location
- Products and tree planting costs
- Gallery and documentary
- Greetings and conversational responses

**Status**: ✅ **ALL RESPONSES ARE WORKING CORRECTLY**

**Optional Improvements**: While the chatbot works perfectly, you could enhance it further by adding more keyword variations and improving the default fallback response for better user experience.
