# swiggy-diagram
Mermaid diagram for Swiggy

# -------- Swiggy -----------
```mermaid
sequenceDiagram
ChatbotEndpoint->>+ShoppingBotWortkflow: Ask product questions
ShoppingBotWortkflow->>+ProductSearchAgent: Tool call to search products
ShoppingBotWortkflow-->>ShoppingBotWortkflow: Save search
ShoppingBotWortkflow->>+RecommendationsAgent: Get product recommendations
ShoppingBotWortkflow-->>ShoppingBotWortkflow: Save recommendations
ShoppingBotWortkflow->>+OrderHistoryDiscoveryAgent: Tool call - discovery - buying history
ShoppingBotWortkflow-->>ShoppingBotWortkflow: Save history
ShoppingBotWortkflow->>+ResponseAgent: Send combined results to agent to generate response
ShoppingBotWortkflow->>+ChatbotEndpoint: Reply with recommendation
```

