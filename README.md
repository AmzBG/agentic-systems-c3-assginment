# Cedar Crumb

A bakery business assistant developed for EECE 503P/798S: Agentic Systems, C3.

Nour answers questions about Cedar Crumb's breads, ingredients, prices, and opening hours using the business profile. The assistant uses Gemini and Gradio, with intent routing, conversation history, tools for customer inquiries and feedback, and a reflection pass that checks each draft before displaying the final reply.

## Project files

```text
business_bot/
├── me/
│   ├── about_business.pdf
│   └── business_summary.txt
├── business_agent.ipynb
└── requirements.txt
```

## Run in Google Colab

1. Open `business_bot/business_agent.ipynb` in Colab and upload the `me` folder with both business documents.
2. Set `PROJECT_DIR` to the folder containing `me` (`/content` by default).
3. Add `GEMINI_API_KEY` in Colab Secrets and enable notebook access.
4. Run the notebook cells in order, then use the Gradio interface. A CPU runtime is sufficient.

Section 12 checks responses, tool calls, contact collection, and reflection. Section 14 displays the saved records. Gemini requests are spaced at least five seconds apart within the notebook runtime.

Cedar Crumb is a fictional business. Inquiries do not confirm orders or availability. Keep API keys and customer logs out of the repository; use sample contact details for demonstrations.
