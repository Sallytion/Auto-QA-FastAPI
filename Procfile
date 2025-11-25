web: uvicorn main:app --host 0.0.0.0 --port $PORT --workers 1

# HEROKU DYNO REQUIREMENTS:
# Minimum: Basic ($7/mo) - 512 MB RAM (may crash under load)
# Recommended: Standard-1X ($25/mo) - 512 MB RAM + better performance
# Best: Standard-2X ($50/mo) - 1 GB RAM (handles ML models comfortably)
#
# Free/Eco dynos ($5/mo) will NOT work - insufficient memory for:
# - ChromaDB
# - sentence-transformers
# - torch
# - LangChain models
#
# To set dyno type: heroku ps:scale web=1:basic
