# Restaurant Voice Agent System

## Responsibility:
A multi-agent voice conversation system for restaurants that handles reservations, takeaway orders, and checkout through natural voice interactions. Features four specialized AI agents that seamlessly transfer conversations while maintaining context.

## Details
- **Framework:** LiveKit Agents
- **Tools Used:** Deepgram STT, Cartesia TTS, OpenAI LLM, Silero VAD
- **AI Model:** GPT-4
- **Date Added:** January 2025
- **License:** MIT
- **Original Source:** [Restaurant Voice Agent System](https://github.com/livekit/agents/blob/main/examples/voice_agents/restaurant_agent.py)

## Install Dependencies
```bash
pip install uv
uv sync
```

## Configure Environment Variables
Copy the example file and add your API keys:

```bash
cp .env.example .env
```

Update `.env` with:
- `LIVEKIT_URL`
- `LIVEKIT_API_KEY`
- `LIVEKIT_API_SECRET`
- `OPENAI_API_KEY`
- `DEEPGRAM_API_KEY`
- `CARTESIA_API_KEY`

## Run Agent
```bash
uv run python main.py console
```

## Agent System

### 🏪 Greeter Agent
Restaurant receptionist that welcomes customers, presents menu (Pizza $10, Salad $5, Ice Cream $3, Coffee $2), and routes to specialized agents.

### 📅 Reservation Agent
Handles dining reservations - collects time, customer name, and phone number.

### 🥡 Takeaway Agent
Processes food orders - takes orders from menu, clarifies requests, confirms details.

### 💳 Checkout Agent
Handles payments - calculates expenses, collects contact info and credit card details.

## Usage Examples

**Getting Started:**
1. Start the agent using `uv run python main.py console`
2. The Greeter Agent will automatically welcome you to the restaurant
3. Say "Hi!" or any greeting to initiate the conversation
4. The agent will then listen to other agent calling it (for example interface agent)
5. Continue your conversation naturally - the system will route you to the appropriate specialized agent

**Making a Reservation:**
1. Say: "I'd like to make a reservation"
2. The system routes you to the Reservation Agent
3. Provide preferred time, name, and phone
4. Confirm details

**Ordering Takeaway:**
1. Say: "I want to order food"
2. The system routes you to the Takeaway Agent
3. Place order from menu
4. Get routed to Checkout Agent for payment
5. Provide payment information and complete transaction

## Creator Details
- **Name:** Ahsen Tahir
- **Contact:** ahsen.t@coralprotocol.org
