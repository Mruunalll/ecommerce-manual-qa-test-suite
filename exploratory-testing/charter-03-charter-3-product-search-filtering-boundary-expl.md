# Charter 3: Product Search & Filtering Boundary Exploration  
**Mission:** Stress-test search and filter interactions for data integrity issues  
**Area:** Shop → Search → Filter → Sort  
**Duration:** 60 minutes  

**Session Notes:**
- SQL injection attempt in search: `' OR '1'='1` — no error, empty results shown ✅
- XSS attempt in search: `<script>alert(1)</script>` — sanitised, shown as plain text ✅
- Very long search string (500 chars) — no crash; truncated gracefully ✅
- Filter + sort + pagination combined → pagination clears filter (BUG-010) ❌
- Price filter with min > max — UI allows it; returns 0 results without explanation ⚠️
- Searched with only spaces — no results, no crash ✅

---
