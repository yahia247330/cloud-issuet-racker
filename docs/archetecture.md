#request flow


##create issue
User → Frontend form → POST /api/issues → API validation → Data layer
 ← Render created issue ← 201 + JSON ←───────────────┘

##view issues 
Page load → GET /api/issues → API → Data layer
 ← Render list ← 200 + JSON array ←───

 ##change status
 Button → PATCH /api/issues/{id}/status → API validation → Data layer
 ← Re-render issue ← 200 + updated JSON ←──────────┘ 

